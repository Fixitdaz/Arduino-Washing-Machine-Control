# Arduino Washing Machine Control

This project simulates a basic washing machine control system using an Arduino Uno. It runs through a short wash program, demonstrating the main stages of a washing machine cycle.

## Table of Contents

- [Features](#features)
- [Hardware Requirements](#hardware-requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Code Explanation](#code-explanation)
- [Future Improvements](#future-improvements)
- [Contributing](#contributing)
- [License](#license)

## Features

- Simulates a complete wash cycle including:
  - Water filling
  - Washing (agitation)
  - Draining
  - Spinning
- Uses a servo motor to simulate the agitator
- Provides status updates via Serial monitor

## Hardware Requirements

- Arduino Uno
- Servo motor (for agitator simulation)
- LEDs or relays (to simulate water valve, drain pump, and main motor)
- Jumper wires
- Breadboard (optional, for prototyping)

## Installation

1. Clone this repository or download the source code.
2. Open the `arduino_washing_machine.ino` file in the Arduino IDE.
3. Connect your Arduino Uno to your computer.
4. Select the correct board and port in the Arduino IDE.
5. Click the upload button to flash the code to your Arduino.

## Usage

1. Set up the circuit according to the pin definitions in the code:
   - Water Valve: Pin 2
   - Drain Pump: Pin 3
   - Main Motor: Pin 4
   - Servo (Agitator): Pin 5
2. Power on your Arduino.
3. Open the Serial Monitor in the Arduino IDE (baud rate: 9600).
4. The washing machine simulation will start automatically and repeat after a short pause.
5. Observe the status updates in the Serial Monitor.

## Code Explanation

The code is structured as follows:

- Pin and time constant definitions
- `setup()` function: Initializes pins and Serial communication
- `loop()` function: Runs the main washing cycle
- `agitateClothes()` function: Simulates the agitation process using a servo motor

The washing cycle consists of four main stages, each with a predefined duration:
1. Filling (1 minute)
2. Washing (5 minutes)
3. Draining (1 minute)
4. Spinning (2 minutes)

## Future Improvements

- Add water level sensors
- Implement temperature control
- Create a user interface for cycle selection
- Add a door lock mechanism
- Incorporate actual motor control instead of simulation

## Contributing

Contributions to this project are welcome! Please fork the repository and submit a pull request with your improvements.

## License

This project is open source and available under the [MIT License](LICENSE).