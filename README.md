# 🐾 Reliable Automated Pet Enclosure

An IoT-based smart pet enclosure designed to close key reliability gaps in existing 
automated pet care systems — built for Sri Lanka's tropical climate, where feeder 
jams and ventilation failures pose real risks to animal health.

## Overview
Most commercial smart cages automate feeding and climate control but don't verify 
whether those actions actually succeed. This project adds **fail-safe detection and 
recovery** on top of standard automation, plus a lightweight wearable for continuous 
pet health tracking — all monitored and controlled remotely through the **Blynk app**.

## Features
- **Feeder Jam Detection** — Load cell + motor current sensing detects blockages, 
  triggers an automatic clearance cycle, and notifies the owner if intervention is needed
- **Fail-Safe Ventilation** — Dual-fan system driven by DHT11 temperature/humidity 
  readings, with automatic failover and alerts on fan malfunction
- **Pet Health Monitoring Collar** — <1oz solar-rechargeable wearable with heart rate 
  and motion sensors (MPU9250), streaming real-time activity/health data via ESP32
- **Remote Monitoring & Control (Blynk App)** — Live dashboard for temperature, 
  humidity, feeder status, fan status, door lock state, water level, pet weight, 
  heart rate, and activity — with manual override for feeding, fans, and door lock

## Hardware
Components            
| ESP32 / ESP32-C3 Mini 
| HX711 + Load Cells   
| DHT11                
| MPU9250            
| Heartbeat Sensor 
| Servo Motors 
| PC Case Fans + Relay 
| Solar Panel + Li-ion Battery 
| Water Level Sensor

## Software / Platform
- Arduino IDE (C/C++ firmware)
- Blynk IoT platform for dashboard, alerts, and remote control

## Results
All core modules — feeder, ventilation, door lock, and health collar — performed 
reliably during testing, with continuous real-time data streaming to the Blynk app. 
The resistive water level sensor showed reduced accuracy at mid-range values; future 
work includes switching to ultrasonic/capacitive sensing and firmware-side filtering.

## Team — Group 07
Department of Information and Communication Technology, Faculty of Technology, 
South Eastern University of Sri Lanka

- M.T. Madapatha — SEU/IS/20/ICT/014 (Group Leader)
- M.B. Jayamanne — SEU/IS/20/ICT/015
- S.T.P. Edirisinghe — SEU/IS/20/ICT/018
- K.P.S.D. Karunarathna — SEU/IS/20/ICT/020
- D.R.S.D.S. Wijayasinghe — SEU/IS/20/ICT/061
