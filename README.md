# Smart Christmas Crib with ESP32

A smart Christmas nativity scene built with ESP32, capable of controlling lighting, music, and a waterfall both locally and remotely.

The system can be managed via:

- physical buttons;
- web interface developed with HTML, CSS, and JavaScript;
- mobile app developed in Flutter;
- Alexa voice assistant.

## Objective
The goal of the project is to integrate electronics, programming, and home automation into a single, easy-to-use system.

## Features
- Turn the nativity scene lights on and off.
- Control the waterfall water pump.
- Play music via SD card.
- Local control via physical buttons.
- Remote control via Wi-Fi.
- Integration with Alexa for voice commands.

## Materials Used
### Hardware
- ESP32
- DFPlayer Mini
- PAM8406 Amplifier
- Relay Modules
- LEDs and String Lights
- Mini Water Pump
- 3W 8Ω Speakers
- Buttons
- Breadboard
- Resistors
- Fuses
- 5V USB-C Power Supply
### Software
- Arduino IDE
- C++
- HTML
- CSS
- JavaScript
- Flutter

## System Architecture

The ESP32 is the heart of the project.
It receives commands from the physical buttons or via Wi-Fi (website, mobile app, or Alexa) and manages the various connected devices.
For music, it communicates with the DFPlayer Mini, which reads MP3 files stored on the SD card.
The audio signal is sent to the PAM8406, which drives the two speakers.
The lights and waterfall pump are controlled via the relay modules.

This way, all control modes use the same centralized logic, ensuring consistent system operation.

## Wiring Diagram

The main connections are:
- common power supply for the ESP32, DFPlayer, amplifier, and relay;
- DFPlayer connected to the ESP32 via UART;
- DFPlayer audio output connected to the PAM8406 amplifier;
- buttons connected to the ESP32's digital inputs;
- relays connected to the ESP32's digital outputs for controlling the lights and pump.

## Images
The complete schematic is included in the Images folder, along with other schematics.

## Code

The code is located in the Arduino folder.

## Video

There are currently no demonstration videos of the finished project. They will be uploaded soon.

## Possible Future Developments
- Light intensity control.
- Automatic programming of switch-on times.
- Management of custom lighting effects.
- System status monitoring via notifications.
- Designing a custom PCB (Printed Circuit Board) to replace the breadboard, making the circuit more compact, reliable, and suitable for permanent use. The Images folder contains a simple, unfinished schematic of what the PCB circuit could look like.

## Author

Emanuele Nassisi
