# MEDIBOX

![alt text](/images/preview.jpeg)

## Table of Contents

1. [Introduction](#introduction)
2. [Problem Statement](#problem-statement)
3. [System Architecture](#system-architecture)
4. [Hardware Components](#hardware-components)
5. [Software Stack](#software-stack)
6. [Implementation Details](#implementation-details)
7. [Testing and Validation](#testing-and-validation)
8. [Results and Analysis](#results-and-analysis)
9. [Challenges and Limitations](#challenges-and-limitations)
10. [Future Work](#future-work)
11. [Conclusion](#conclusion)
12. [Authors](#authors)

## Introduction

MediBox is an **automated medicine dispensing and health monitoring system** developed as a final-year project in the Department of Electrical and Electronic Engineering, University of Ibadan, Nigeria by [Areo Benjamen](https:linkedin.com/in/areo-benjamen) & [Ajiboye Ajibola](###) under the supervision of [Dr. K.O Odeyemi](https://www.linkedin.com/in/kehinde-odeyemi-751b171b/).

The system is designed to improve medication adherence by alerting users when their medication is due, dispensing the correct dosage, and monitoring key health parameters.

MediBox aims to enhance patient care, particularly for individuals with chronic illnesses or those requiring strict medication schedules.  

## Problem Statement

In contemporary healthcare, medication non-adherence remains a significant challenge, particularly among the elderly and individuals with chronic illnesses. The World Health Organization reports that nearly 50% of patients with chronic diseases do not adhere to their prescribed medication regimens, leading to severe health complications and increased healthcare costs (WHO, 2021). This issue not only jeopardizes patient health outcomes but also strains healthcare systems, with medication non-adherence costing the U.S. healthcare system an estimated $290 billion annually (New England Healthcare Institute, 2009).

## Objectives

The objectives of this project are to:

- design, 3D-print, and laser-cut the models of the physical components of the medicine dispenser which contains medicine containers, tubes, solenoid holders, and other casings;

- interface the mechanical components with the electronic unit (microcontroller & power source) to dispense the medicine containers at scheduled times;

- integrate the health monitoring sensors into the microcontroller; and
- develop a web-based software platform for remote data monitoring and sync with the microcontroller via Wifi.

## System Architecture

![Architecture Block Diagram](<images/architecture.png>)

The block diagram above describes the overall architecture of the sytem. The Microcontroller(ESP32) serves as the brain of the system, regulating all other mechanisms including the health monitoring system and the drug dispensing.

## Hardware Components

1. **JF-0530B 12V Linear Solenoids** : Solenoids are electromagnetic actuators used in the dispensing mechanism. When activated, they generate a linear motion that pushes medicine vials out of the storage compartment

    <img src="solenoids.jpeg" alt="linear solenoids" width="200" height="200">

2. **GY-MAX30102 Heart Rate/Oxygen Concentration Sensor Module** : This sensor module is used for real-time monitoring of heart rate and blood oxygen levels. It operates using an optical method, measuring changes in blood volume through infrared and red light absorption.

    <img src="images/hardware components/max30102.png" alt="Heart Rate/Oxygen Concentration Sensor Module" width="200" height="200">

3. **PCF8574T IO Expansion Board** : This board extends the ESP32’s I/O capabilities, enabling additional connections for components such as buttons, LEDs, and additional sensors.

    <img src="images/hardware components/expansion.png" alt="expansion board" width="200" height="200">

4. **Bi-Directional Logic Level Converter** : The logic level converter ensures compatibility between components operating at different voltage levels, particularly between the ESP32 (3.3V logic) and other peripherals requiring 5V logic

     <img src="images/hardware components/level-converter.png" alt="expansion board" width="200" height="200">


## Software Stack
## Software Stack

The software stack for MediBox comprises:

- **Frontend**: Built using React, providing an intuitive and responsive user interface for remote monitoring and interaction.
- **Backend**: Developed with Node.js, handling API requests, data processing, and communication with the microcontroller.
- **Deployment**: Hosted on an AWS EC2 instance, ensuring scalability, reliability, and secure access to the system.

This architecture enables seamless integration between the hardware components and the web-based platform.

<!-- ## Implementation Details

Explain the step-by-step process of building the system, including circuit design, firmware development, and integration with the software.

## Testing and Validation

Describe the testing methodology, test cases, and validation processes employed to ensure system reliability.

## Results and Analysis

Present the results obtained from the system's operation, including data analysis and performance metrics.

## Challenges and Limitations

Discuss the challenges faced during development and the limitations of the current system.

## Future Work

Highlight potential improvements and future enhancements for the system.

## Conclusion

Summarize the key findings and achievements of the project. -->

## Authors

- [AREO BENJAMEN](https:linkedin.com/in/areo-benjamen)
- [AJIBOYE AJIBOLA]()

## Supervisor  

- [Dr. K.O ODEYEMI](https://www.linkedin.com/in/kehinde-odeyemi-751b171b/)
