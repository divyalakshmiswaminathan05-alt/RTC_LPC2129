# ⏰ RTC Digital Clock using LPC2129

## 📌 Overview

This project implements a **Real-Time Clock (RTC) based digital clock** using the LPC2129 microcontroller and DS1307 RTC module. The system reads time using I2C communication, converts it from BCD to decimal, and displays the real-time output on a 16×2 LCD and a UART virtual terminal.

---

## ⚙️ Features

* Real-time clock using **DS1307 RTC**
* I2C communication interface (P0.2 – SCL, P0.3 – SDA)
* Dual display output (LCD + UART)
* BCD to decimal conversion for accurate display
* Continuous real-time updates
* Proteus-based simulation

---

## 🧰 Components Used

* LPC2129 Microcontroller
* DS1307 RTC Module
* 16×2 LCD Display
* 32.768 kHz Crystal Oscillator
* Pull-up Resistors (4.7kΩ for I2C lines)
* Virtual Terminal (Proteus)
* Power Supply

---

## 🔌 Circuit Connections

### 🔹 I2C Interface

* **P0.2 → SCL (Clock)**
* **P0.3 → SDA (Data)**

### 🔹 LCD Interface

* Data Pins → P1.16 to P1.23
* RS → P1.24
* E → P1.26
* RW → GND

### 🔹 UART Interface

* TXD0 → P0.0
* RXD0 → P0.1

---

## 🚀 Working Principle

1. The DS1307 RTC maintains real-time using a crystal oscillator.
2. LPC2129 communicates with RTC via I2C protocol.
3. RTC provides time in BCD format.
4. Microcontroller converts BCD to decimal.
5. Time is displayed on LCD and transmitted via UART.

---

## ▶️ How to Run

1. Open the project in **Keil µVision**
2. Compile and generate the `.hex` file
3. Load the `.hex` file into **Proteus simulation**
4. Run the simulation
5. Observe time on LCD and Virtual Terminal

---

## 📷 Output

* LCD displays real-time clock in `HH:MM:SS` format
* Virtual Terminal shows the same time continuously

---

## 📚 Future Enhancements

* Date display (DD/MM/YYYY)
* Alarm and timer features
* 12-hour format with AM/PM
* IoT integration (Wi-Fi / Bluetooth)
* Mobile app interface

---

## 💡 Key Learnings

* I2C communication in embedded systems
* RTC interfacing and time management
* LCD and UART integration
* Handling BCD data formats
* Debugging hardware-software interaction

---

## 👩‍💻 Author

**Divya Lakshmi S**
