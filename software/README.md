# Czech Rocket Challenge 2025 - Rocket Control System

This repository contains C++ software for the Czech Rocket Challenge (CRC) competition, designed to run on Raspberry Pi Pico hardware and interface with the GRAGAS_MAY24 rocket engine.

## Project Overview

This software provides control systems for rocket launches as part of the Czech Rocket Challenge competition. It handles sensor data processing, flight control algorithms, and engine management for the GRAGAS_MAY24 rocket engine.

## Hardware Components

- **Microcontroller**: Raspberry Pi Pico
- **Rocket Engine**: GRAGAS_MAY24
- **Sensors**: (List your specific sensors here)
- **Additional Hardware**: (List any other hardware components)

## Software Requirements

- C++ compiler (compatible with Raspberry Pi Pico)
- Raspberry Pi Pico SDK
- CMake (version 3.13 or higher)
- (Any other dependencies)

## Installation

### Setting up the Development Environment

1. Clone this repository:
```plaintext
git clone https://github.com/redfox-studios/crc-rocket-software.git
cd crc-rocket-software
```

2. Install the Raspberry Pi Pico SDK:
```
git clone https://github.com/raspberrypi/pico-sdk.git
cd pico-sdk
git submodule update --init
cd ..
```

3. Set the PICO_SDK_PATH environment variable:
```plaintext
export PICO_SDK_PATH=/path/to/pico-sdk
```

4. Build the project:
```plaintext
mkdir build
cd build
cmake ..
make
```

## Usage

### Uploading to Raspberry Pi Pico

1. Connect your Raspberry Pi Pico to your computer while holding the BOOTSEL button.
2. Release the button after connecting.
3. Copy the generated `.uf2` file to the Pico drive:
```plaintext
cp rocket_control.uf2 /media/redfox-studios/RPI-RP2/
```

### Configuration

The system can be configured by modifying the `config.h` file:

- Engine parameters
- Sensor calibration
- Flight control settings
- Safety thresholds

### Pre-flight Checklist

1. Ensure all connections are secure
2. Run the built-in diagnostics: (instructions)
3. Verify sensor readings
4. Perform engine pre-check

## Project Structure

```plaintext
├── src/                  # Source files
│   ├── main.cpp          # Entry point
│   ├── engine/           # Engine control code
│   ├── sensors/          # Sensor interface code
│   └── flight/           # Flight control algorithms
├── include/              # Header files
├── lib/                  # External libraries
├── tests/                # Test code
└── docs/                 # Documentation
```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Czech Rocket Challenge organization
- Ivan Gábriš
- Martin Paluš
- Michal Flaška
- Martin Weis

## Contact

- Team Name: RedFox
- Email: (Your contact email)
