# Emerging-Sys-Arch-Tech
Emerging System Architecture and Technology 

# CS 350 – Emerging Systems Architectures and Technologies

## Course Overview

This repository contains work completed throughout **CS 350: Emerging Systems Architectures and Technologies** at Southern New Hampshire University. The course focused on embedded systems and the relationship between software and physical hardware.

Throughout the course, I used a **Raspberry Pi 4B and Python** to develop increasingly complex embedded applications. Individual assignments introduced concepts such as GPIO control, pulse-width modulation (PWM), hardware interrupts, state machines, displays, sensors, I2C, and UART communication. These concepts were eventually combined into a complete embedded system for the final project.

## Technologies and Concepts

Some of the primary technologies and concepts explored throughout CS 350 include:

* Raspberry Pi 4B
* Python
* GPIO and GPIOZero
* Digital input and output
* Pulse-width modulation (PWM)
* Hardware interrupts
* State-machine design
* I2C communication
* UART serial communication
* Temperature and humidity sensors
* 16x2 LCD displays
* LEDs and physical push buttons
* Embedded system architecture
* Hardware/software integration
* IoT and cloud-connected systems
* Debugging and hardware troubleshooting

## Hardware and Software Development

One of the main focuses of this course was learning how software can interact with physical hardware.

Early assignments introduced basic GPIO operations by controlling LEDs connected to the Raspberry Pi. From there, I worked with PWM to control LED brightness and create fading effects. This provided experience controlling hardware through software rather than simply turning a GPIO output on or off.

As the circuit became more complex, physical buttons were incorporated into the system. These exercises introduced event-driven programming and hardware interrupts. Instead of continuously checking whether a button had been pressed, the program could respond to GPIO events and perform an appropriate action.

State machines were also introduced as a way to organize the behavior of embedded applications. Using clearly defined states and transitions made it easier to control increasingly complex hardware without relying on large amounts of conditional logic.

## Sensors and Displays

Later assignments introduced additional peripherals, including a **16x2 LCD display** and an **AHT20 temperature and humidity sensor**.

The AHT20 communicates with the Raspberry Pi through the **I2C communication protocol**. Python code was used to retrieve sensor measurements and process the information for use within the application.

The LCD provided a way for the embedded system to communicate information directly to the user. Integrating the sensor and display demonstrated how an embedded application can collect information from one hardware peripheral, process that information through software, and provide output through another peripheral.

## Communication Protocols

CS 350 also provided experience working with several communication methods commonly found in embedded systems.

**I2C** was used to communicate with the temperature sensor, while **UART serial communication** was incorporated into the final system to simulate sending information from an embedded device to an external server.

Working with these protocols helped demonstrate that embedded systems frequently depend on multiple communication interfaces operating together within the same application.

## Final Smart Thermostat Project

The final project brought together many of the concepts developed throughout the course by creating a prototype **smart thermostat**.

The thermostat uses an AHT20 sensor to monitor room temperature and a state machine to manage three operating modes:

* **Off**
* **Heat**
* **Cool**

Three physical buttons allow the user to change the operating mode and increase or decrease the temperature set point. Red and blue PWM LEDs represent heating and cooling activity, while a 16x2 LCD displays the date, time, current temperature, operating state, and temperature set point.

The system also uses UART communication to periodically transmit thermostat information in a comma-delimited format, simulating communication between the embedded device and a remote server.

The project demonstrated how GPIO, PWM, interrupts, I2C, UART, state machines, sensors, displays, and multithreaded software can be combined into a single embedded application.

## What I Learned

The most significant lesson I gained from CS 350 was a better understanding of the relationship between **hardware and software**. Before working with embedded systems, software development was primarily something I associated with applications running entirely within a computer. This course demonstrated how software can interact with and control devices in the physical world.

I also gained valuable troubleshooting experience. When working with embedded systems, a problem is not necessarily caused by the code. Wiring, GPIO assignments, component orientation, communication interfaces, and hardware configuration can all affect application behavior. Testing individual components before combining them into a larger system proved to be an effective way to identify and resolve problems.

The course also reinforced the importance of writing organized and modular code. State machines, functions, classes, and event-driven programming helped make increasingly complicated hardware behavior easier to understand and maintain.

## Emerging Systems and IoT

Another important part of the course was examining how embedded systems can evolve into connected **Internet of Things (IoT)** devices.

The Raspberry Pi provided an effective development platform for prototyping, but production embedded systems must also consider factors such as processor architecture, available RAM and Flash storage, peripheral support, power consumption, networking capabilities, cost, and scalability.

The final project explored how a prototype thermostat could eventually communicate with cloud infrastructure through Wi-Fi. This demonstrated how embedded hardware can serve as the foundation for larger connected systems that collect, transmit, and analyze real-world information.

## Reflection

CS 350 provided practical experience that connected software development concepts with physical computing. Each assignment built on previous work, progressing from basic LED control to a complete system involving multiple inputs, outputs, sensors, communication protocols, and software components.

The hands-on nature of the course helped strengthen my understanding of Python programming, event-driven development, state machines, communication protocols, hardware architecture, and troubleshooting.

The skills developed throughout this course provide a foundation for continued work with **embedded systems, IoT devices, hardware/software integration, and emerging computing technologies**.
