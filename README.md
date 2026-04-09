# 🔥 Fire Alert System with Real-Time Occupancy Monitoring

## 📌 Overview

This project is an embedded safety system built using ESP32 that detects fire and monitors the number of people present in a room in real time. In case of fire, it triggers an alert using a buzzer, sends a message via Bluetooth, and notifies a mobile number using a GSM module. The system operates independently without requiring an internet connection.

---

## 🚀 Features

* 🔥 Fire detection using flame sensor
* 👥 Real-time people counting using IR sensors
* 📱 SMS alert using GSM module (no internet required)
* 📶 Bluetooth communication with mobile devices
* 🔔 Buzzer alert during emergency
* ⚡ Efficient state machine for accurate counting

---

## 🛠️ Components Used

* ESP32 Microcontroller
* Flame Sensor
* IR Sensors (2 units)
* GSM Module (SIM800/SIM900)
* Buzzer
* Connecting wires & power supply

---

## ⚙️ Working Principle

* The flame sensor continuously monitors fire presence.
* If fire is detected:

  * Buzzer is activated
  * Alert message is sent via Bluetooth
  * SMS is sent with current occupancy count using GSM network
* IR sensors track entry and exit:

  * Entry → increments count
  * Exit → decrements count
* A state machine ensures accurate movement detection and avoids false counts.

---

## 📲 GSM Alert Format

Example SMS:
FIRE ALERT! People inside: 5

---

## 🎯 Applications

* Smart classrooms
* Office safety systems
* Industrial monitoring
* Public building evacuation systems

---

## 📈 Future Improvements

* Integration with local alarm systems
* LCD display for live occupancy count
* Battery backup for power failure scenarios
* Enhanced sensor accuracy
