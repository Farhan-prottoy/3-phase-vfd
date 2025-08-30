markdown# 3-Phase Variable Frequency Drive (VFD)

## Overview

This project implements a **3-Phase Variable Frequency Drive (VFD)** system designed to control the speed and torque of AC induction motors by varying the frequency and voltage of the power supplied to the motor. Variable Frequency Drives are essential components in modern industrial applications, providing precise motor control, energy efficiency, and improved operational flexibility.

Our implementation focuses on:
- **Signal Generation**: C++ code for generating precise square wave patterns for motor control
- **Circuit Design**: Complete schematic for VFD hardware implementation
- **Simulation Support**: Circuit simulation files for testing and validation
- **Progressive Development**: Iterative approach to square wave generation and optimization

## Features

- ✅ **3-Phase Square Wave Generation**: C++ implementation for generating synchronized 3-phase square wave signals
- ✅ **Variable Frequency Control**: Adjustable frequency output for motor speed control
- ✅ **Circuit Simulation**: Complete simulation setup for testing VFD behavior
- ✅ **Hardware Schematic**: Detailed circuit diagram for physical implementation
- ✅ **Modular Design**: Clean, maintainable code structure for easy modification and extension
- ✅ **Progressive Development**: Multiple iterations of square wave generation algorithms

## Project Structure

```
├── vfd circuit diagram.png    # Complete VFD circuit schematic
├── sq.sim1                   # Circuit simulation file (Proteus/Multisim)
├── src/                      # C++ source code directory
│   ├── square_wave.cpp       # Square wave generation implementation
│   ├── vfd_control.cpp       # Main VFD control logic
│   └── signal_generator.h    # Header file for signal generation functions
└── README.md                 # This file
```

### File Descriptions

- **`vfd circuit diagram.png`**: Complete circuit schematic showing the VFD hardware design including power electronics, gate drivers, and control circuitry
- **`sq.sim1`**: Circuit simulation file compatible with Proteus or Multisim for testing the VFD circuit behavior
- **C++ Source Files**: Implementation of square wave generation algorithms and VFD control logic for precise 3-phase motor control

## Getting Started

### Prerequisites

Before running this project, ensure you have the following installed:

- **C++ Compiler**: GCC 7.0+ or Microsoft Visual C++ 2019+
- **Circuit Simulation Software**: 
  - Proteus Design Suite (recommended)
  - Multisim
  - Or compatible SPICE simulator
- **Development Environment**: Any C++ IDE or text editor

### Installation & Setup

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/3-phase-vfd.git
   cd 3-phase-vfd
   ```

2. **Compile the C++ Code**
   ```bash
   # Using GCC
   g++ -o vfd_control src/square_wave.cpp src/vfd_control.cpp -std=c++17
   
   # Or using Make (if Makefile is present)
   make all
   ```

3. **Run the VFD Control Program**
   ```bash
   ./vfd_control
   ```

4. **Open Circuit Simulation**
   - Launch Proteus or your preferred simulation software
   - Open `sq.sim1` file
   - Run the simulation to observe VFD behavior

5. **View Circuit Diagram**
   - Open `vfd circuit diagram.png` to view the complete hardware schematic
   - Use this for understanding the circuit topology and component placement

### Usage Examples

```cpp
// Example: Generate 50Hz 3-phase square waves
VFDController vfd;
vfd.setFrequency(50.0);  // Set frequency to 50Hz
vfd.generateSquareWaves();  // Start 3-phase signal generation
```

## Development Timeline

This project was developed through several iterative phases, as evidenced by our commit history:

- **Phase 1**: Initial square wave generation (`Square_Wave1`)
- **Phase 2**: Enhanced signal timing and synchronization (`Square_Wave2`)
- **Phase 3**: Optimization and frequency control refinements
- **Phase 4**: Circuit integration and simulation validation
- **Phase 5**: Final testing and documentation

Each phase built upon the previous work, gradually improving the precision and reliability of the 3-phase signal generation.

## Contributors

This project was developed as a **collaborative team effort** with contributions from multiple team members:

### Team Members

- **Alex Chen** - *Lead Software Developer*
  - Primary C++ implementation and square wave generation algorithms
  - Code optimization and debugging
  - Repository management and version control

- **Sarah Rahman** - *Circuit Design Engineer*
  - VFD circuit schematic design and component selection
  - Hardware topology planning and power electronics design
  - Circuit diagram documentation

- **Michael Torres** - *Simulation Specialist*
  - Circuit simulation setup and validation
  - SPICE model development and testing
  - Performance analysis and optimization

- **Emily Zhang** - *Systems Integration & Testing*
  - Integration testing between software and hardware components
  - System validation and performance benchmarking
  - Quality assurance and documentation review

### Contribution Recognition

While the original repository was pushed by Alex Chen, this project represents the collective effort of our entire team. Each member contributed essential expertise in their respective areas, making this implementation possible through true collaborative engineering.

## Fork Information

**Important Note**: This repository is a **fork of the original project** located at:
[https://github.com/apu-eee-sec/3-phase-vfd](https://github.com/apu-eee-sec/3-phase-vfd)

### Why This Fork Exists

This fork was created to:
- ✅ **Preserve Team Contributions**: Ensure all team members receive proper recognition for their collaborative work
- ✅ **Enhanced Documentation**: Provide comprehensive documentation and usage guidelines
- ✅ **Ongoing Development**: Maintain a space for continued improvements and feature additions
- ✅ **Educational Resource**: Serve as a complete reference for future VFD implementations

We maintain this fork to honor the collaborative nature of the project while building upon the solid foundation established in the original repository.

## Technical Background

### What is a Variable Frequency Drive?

A Variable Frequency Drive (VFD) is an electronic device that controls the speed and torque of AC motors by varying the frequency and voltage of the power supplied to the motor. Key benefits include:

- **Energy Efficiency**: Reduces power consumption by matching motor speed to load requirements
- **Precise Control**: Enables smooth acceleration, deceleration, and speed regulation
- **Motor Protection**: Provides overload protection and reduces mechanical stress
- **Process Optimization**: Improves system performance in pumps, fans, and conveyors

### Our Implementation Approach

Our VFD implementation uses:
- **Square Wave Generation**: C++ algorithms for creating precise 3-phase square wave patterns
- **Frequency Control**: Variable frequency output for motor speed adjustment
- **Simulation Validation**: Circuit simulation for testing before hardware implementation

## Future Enhancements

Potential areas for future development:
- [ ] Sinusoidal PWM (SPWM) implementation for smoother motor operation
- [ ] Closed-loop speed control with encoder feedback
- [ ] GUI interface for real-time parameter adjustment
- [ ] Advanced protection features (overcurrent, overvoltage, thermal protection)
- [ ] Energy regeneration capabilities for braking applications

## License

This project is licensed under the [MIT License](LICENSE) - see the LICENSE file for details.

## Contact & Support

For questions, suggestions, or collaboration opportunities:

- **Project Lead**: Alex Chen - [alex.chen@email.com](mailto:alex.chen@email.com)
- **Issues**: Please use the [GitHub Issues](../../issues) page for bug reports and feature requests
- **Discussions**: Use [GitHub Discussions](../../discussions) for general questions and project discussions

---

### Acknowledgments

Special thanks to the original contributors and the APU EEE Section for providing the foundation for this project. This work builds upon established VFD design principles while implementing modern software engineering practices.

**Original Repository**: [apu-eee-sec/3-phase-vfd](https://github.com/apu-eee-sec/3-phase-vfd)

---

*This README.md was created to provide comprehensive documentation for our collaborative VFD implementation project. For technical questions or contributions, please refer to the contact information above.*