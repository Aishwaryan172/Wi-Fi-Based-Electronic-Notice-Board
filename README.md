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

Required Components
P10 LED Display Module (HUB12) – Displays text and animations.
Wi-Fi Controller Card (HD-W00) – Controls the LED display via Wi-Fi.
Power Supply (SMPS, 5V 40A recommended) – Powers both the HD-W00 and P10 LED panel.
Mobile Phone – Used to send messages via the Serial Bluetooth Terminal App.

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
   
## Methodology
1. Establish a Wi-Fi network connecting the mobile application to the system.
2. Verify user authorization using password authentication.
3. Save the transmitted message in the memory of the Wi-Fi module.
4. Retrieve messages using specific commands and send them to the display board.
5. Display messages on the P10 LED display.
---

### Setup Diagram
![Setup Diagram](Set%20up%20Diagram.png)  
**Fig 3: Setup Diagram**
1. Wi-Fi antenna(1): Connect the computer or mobile phone through Wi-Fi to send
parameters and programs.
2. Power connector(2): Connect +5V power supply.
3. S1 test button(3): Click to switch screen test status.
4. Port 7(4): Connect the brightness sensor.
5. S2 Connect the point switch(5):switch to next program, the timer starts, count plus.
6. S3 Connect the point switch(6): Switch the previous program, timer reset, count
down.
7. S4 Connect the point switch(7): Program control, timing pause, count reset.
8. HUB12(8): Connect the display.
9. Port5(9): Connect the temperature/humidity sensor.
10. Port11(10): Connect the IR, by remote control.

### Architecture
![Architecture](Architecture.png)  
**Fig 2: Architecture of Wireless Notice Board**

---
Circuit Connection Explanation
1️⃣ Power Connections (SMPS → HD-W00 & P10 LED Module)
    Connect +5V from the SMPS to the VCC (5V) terminals of both:
    P10 LED module (5V input terminal).
    HD-W00 controller card (5V input terminal).
    Connect GND from the SMPS to the GND terminals of both:
    P10 LED module (GND terminal).
    HD-W00 controller card (GND terminal).

2️⃣ Data (Signal) Connections (HD-W00 → P10 LED Panel via HUB12 Port)
    Use the ribbon cable to connect the HD-W00 controller to the P10 LED module:
    Insert one end into the HD-W00 controller’s HUB12 port.
    Insert the other end into the P10 LED module’s HUB12 port.

  Steps to Set Up the System
  Step 1: Powering Up the System
  Ensure all connections are correct before switching on the SMPS power supply.
  
  Turn on the SMPS, and both the HD-W00 controller and P10 LED module should power up.
  
  The HD-W00 LED indicator should start blinking, indicating that it's ready to connect via Wi-Fi.
  
  Step 2: Connecting to the HD-W00 via Wi-Fi
  On your mobile phone, enable Wi-Fi.
  
  Look for the Wi-Fi network broadcasted by the HD-W00 controller (e.g., LED-WIFI-XXXX).
  
  Connect to this Wi-Fi network (no password required by default).
  
  Step 3: Sending Messages via Serial Bluetooth Terminal App
  Install the "Serial Bluetooth Terminal" app from the Google Play Store.
  
  Open the app and go to Devices.
  
  Select HD-W00 from the available devices list.
  
  Tap Connect, and the status should change to "Connected".
  
  Now, go to the terminal section of the app and type a message (e.g., "HELLO WORLD").
  
  Tap Send, and the message should appear on the P10 LED display!
  
  ✅ Final Working of the System
  The HD-W00 controller receives the message from the Serial Bluetooth Terminal app.
  
  It processes the message and sends it to the P10 LED module via the HUB12 interface.
  
  The P10 LED module displays the message in real time.
  
  Users can update the message anytime using the app without reprogramming the hardware.
  
  🎯 Key Features of This Setup
  ✅ No need for additional microcontrollers like Arduino – The HD-W00 directly controls the display.
  ✅ Wireless message updating – No need to connect cables; just use the app.
  ✅ Works with a single P10 panel or multiple chained panels.
  ✅ Simple and cost-effective solution for LED display boards.




