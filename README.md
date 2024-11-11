# Wi-Fi Based Wireless Electronic Notice Board

A project to design and implement a wireless electronic notice board using Wi-Fi technology. The system facilitates sending messages through a mobile application and displaying them on an LED display.

---

## Table of Contents
- [Introduction](#introduction)
- [Objectives](#objectives)
- [Hardware Requirements](#hardware-requirements)
- [Software Requirements](#software-requirements)
- [System Design](#system-design)
  - [Block Diagram](#block-diagram)
  - [Architecture](#architecture)
  - [Setup Diagram](#setup-diagram)
- [Methodology](#methodology)

---

## Introduction
1. Digital advertisements have become popular in shopping malls, supermarkets, and airports.  
2. Mobile phones and related technologies are an integral part of modern life.  
3. The project aims to leverage Wi-Fi-enabled mobile phones to send and display messages on a digital board.  
4. This system reduces manual effort and enables remote management of notice boards.

---

## Objectives
1. Develop a wireless notice board capable of accessing messages via a Wi-Fi module.
2. Replace conventional notice boards with wireless digital displays.
3. Design a system that can be deployed universally with Wi-Fi connectivity.
4. Create a low-power, user-friendly notice board solution.

---

## Hardware Requirements
- Single Color Wi-Fi Control Card  
- RTC (Real-Time Clock)  
- Temperature Sensor  
- Power Source  
- P10 LED Display  

---

## Software Requirements
- **LED Art App** or **Computer** for controlling the display.

---

## System Design

### Block Diagram
![Block Diagram](Block%20Diagram.png)  
**Fig 1: Block Diagram of Wireless Notice Board**

#### Components:
1. **Mobile Phone**: Hosts the `LED Art App` to send messages.  
2. **Wi-Fi Controller Card**: Receives messages via Wi-Fi.  
3. **Power Supply**: Powers the Wi-Fi controller card and LED display.  
4. **P10 LED Display**: Displays messages sent from the mobile application.  

---

### Architecture
![Architecture](Architecture.png)  
**Fig 2: Architecture of Wireless Notice Board**

---

### Setup Diagram
![Setup Diagram](Set%20up%20Diagram.png)  
**Fig 3: Setup Diagram**

#### Key Features:
- **Wi-Fi Antenna**: Connects mobile phone/computer to the system.  
- **Power Connector**: Supplies +5V power.  
- **Buttons and Ports**:
  - Port 7: Brightness sensor.
  - Port 5: Temperature/humidity sensor.
  - Port 11: IR remote control.

---

## Methodology
1. Establish a Wi-Fi network connecting the mobile application to the system.
2. Verify user authorization using password authentication.
3. Save the transmitted message in the memory of the Wi-Fi module.
4. Retrieve messages using specific commands and send them to the display board.
5. Display messages on the P10 LED display.

---

## Project Highlights
- **Easy to operate**: Controlled via a mobile app.
- **Versatile deployment**: Works in various locations with Wi-Fi connectivity.
- **Energy efficient**: Designed for low power consumption.

