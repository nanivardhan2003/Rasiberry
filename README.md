
## Overview

This project is designed to encourage better ergonomics while using a laptop by monitoring the distance of a user's face from the laptop. If the user’s face is closer than 30 cm to the laptop screen, a buzzer will sound, alerting the user to sit back and maintain a healthier distance. The system uses an ultrasonic sensor to measure the distance and a buzzer to provide the alert.

## Features

- **Distance Monitoring**: Continuously monitors the distance between the user’s face and the laptop using an ultrasonic sensor.
- **Buzzer Alert**: Sounds a buzzer if the user is detected within 30 cm of the laptop, reminding them to sit back.
- **Flexible Sensor Integration**: Uses an analog-to-digital converter (ADC) for additional sensor input (like a flex sensor) for further customization.

## Components

- **Ultrasonic Sensor (HC-SR04)**: Used to measure the distance between the user's face and the laptop.
- **Buzzer**: Alerts the user when they are too close to the laptop.
- **Flex Sensor (optional)**: Could be used for additional ergonomic feedback.
- **Microcontroller**: Such as Raspberry Pi Pico, used to control the components.

## Prerequisites

- **Microcontroller** (e.g., Raspberry Pi Pico)
- **Ultrasonic Sensor** (HC-SR04)
- **Buzzer**
- **Optional**: Flex Sensor and additional wires for connections

## Circuit Diagram

1. **Ultrasonic Sensor**: Connect the trigger pin to GPIO 21 and the echo pin to GPIO 20.
2. **Buzzer**: Connect to GPIO 8.
3. **Flex Sensor**: Connect to ADC pin 26.
4. **Switch**: Connect to GPIO 9 for enabling/disabling the buzzer.

## Usage

1. **Power the Circuit**: Connect your microcontroller to a power source.
2. **Start Monitoring**: The system will begin to monitor the distance as soon as it is powered on.
3. **Listen for Alerts**: If you hear the buzzer, adjust your sitting position to be at least 30 cm away from the laptop screen.

## Conclusion

This project helps promote better posture and ergonomic habits by providing real-time feedback when a user is too close to their laptop screen. With simple components and code, it’s an effective solution for encouraging healthy computing habits.

## Future Enhancements

- **Additional Sensors**: Integrate more sensors to monitor other aspects of ergonomics, like seating position.
- **Smart Alerts**: Use more sophisticated alert systems, like gentle vibrations or visual indicators, instead of a buzzer.
