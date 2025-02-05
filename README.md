# Embedded System for Hazardous Gas and Fire Detection

## Overview
This project aims to enhance safety in industrial and domestic environments by developing an embedded system for detecting hazardous gas leaks and fire. The system is built using an STM32 microcontroller, a gas sensor (MQ9), and a flame detector. It provides real-time alerts to warn users about potential dangers, ensuring a rapid response to mitigate risks.

## Features
- *Real-time Gas and Fire Detection*: Uses MQ9 gas sensor for detecting Carbon Monoxide (CO) and Methane (CH4) and a flame sensor for fire detection.
- *STM32-Based Embedded System*: Efficiently processes sensor data and triggers alerts.
- *Visual and Audible Alerts*: LEDs and a buzzer provide immediate warnings.
- *LCD Display*: Displays system status and detected hazards.
- *Prototyping and Testing*: Simulated in Proteus and tested in real-life scenarios.

## System Components
- *STM32 Nucleo-F401RE*: Microcontroller used for data processing and control.
- *MQ9 Gas Sensor*: Detects hazardous gases (CO and CH4).
- *Flame Sensor*: Detects fire presence.
- *LCD Display*: Shows system messages.
- *Buzzer & LEDs*: Alert users to gas leaks or fire.

## Circuit Simulation and Prototype Implementation
- *Simulation*: Designed and tested using Proteus software.
- *Prototype Development*: Hardware assembled and tested in real-world conditions.
- *Calibration and Testing*: Sensors calibrated for accuracy and tested across multiple scenarios.
- *Data Acquisition and Processing*: Implemented using STM32CubeIDE.

## Simulation
[![video](https://github.com/Nada-Abidii/Gas-and-fire-detection/blob/master/simulation.png)](https://drive.google.com/file/d/1qNoo924DbBA1huwt8rrZYbGedHFFFuWO/view?usp=drive_link)

## Scenarios
### 1️⃣ Safe Condition (No Gas, No Fire)
- ✅ *Green LED ON* (Indicates safety)  
- ❌ *Red LED OFF*  
- ❌ *Buzzer OFF*  
- 📟 *LCD displays:* "Safe" 
![demo](/1st_scenario.png)
### 2️⃣ Gas Leak Detected (Gas but No Fire)
- ❌ *Green LED OFF*  
- 🔴 *Red LED ON* (Indicates gas presence)  
- 🔊 *Buzzer ON* (Warning sound if gas percentage > 50%)  
- 📟 *LCD displays:* "Gas"  
![demo](/2nd_scenario.png)
### 3️⃣ Fire Detected (Fire but No Gas)
- ✅ *Green LED ON* (No gas detected)  
- ❌ *Red LED OFF*  
- 🔊 *Buzzer ON* (Fire warning)  
- 📟 *LCD displays:* "Fire"  
![demo](/3rd_scenario.png)
### 4️⃣ Gas and Fire Detected
- ❌ *Green LED OFF*  
- 🔴 *Red LED ON*  
- 🔊 *Buzzer ON* (Indicates extreme danger)  
- 📟 *LCD displays:* "Gas and Fire"  
![demo](/4th_scenario.png)

