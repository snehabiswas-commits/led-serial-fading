# led-serial-fading
An embedded systems mini-project using ESP32 and PlatformIO to demonstrate serial communication, PWM-based LED fading, and real-time brightness control on GPIO 2
# ESP32 Serial LED Fading

A simple ESP32 project built in PlatformIO to control LED brightness through the Serial Monitor using PWM on **GPIO 2**. The user enters a value from **0 to 255**, and the LED brightness updates in real time.

## Overview
This project demonstrates the basics of **serial communication**, **PWM-based brightness control**, and **GPIO output handling** on an ESP32. It is designed as a beginner-friendly embedded systems project to show how software commands can directly control hardware behavior.

## Features
- Serial-controlled LED brightness
- PWM output on **GPIO 2**
- Brightness range from **0 to 255**
- Real-time LED intensity update
- Built using **PlatformIO** and **ESP32**

## Hardware Required
- ESP32 development board
- LED
- 220Ω resistor
- Breadboard and jumper wires
- USB cable

## Circuit Connection
- **LED anode (+)** → **GPIO 2**
- **LED cathode (-)** → **220Ω resistor** → **GND**

> If your ESP32 board already has an onboard LED connected to GPIO 2, an external LED may not be necessary.

## How It Works
The ESP32 reads a brightness value from the Serial Monitor and uses **PWM (Pulse Width Modulation)** to adjust the LED intensity:
- `0` → LED OFF
- `255` → Maximum brightness
- Intermediate values → proportional brightness.
