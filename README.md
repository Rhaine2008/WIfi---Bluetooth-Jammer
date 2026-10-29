# Wi-Fi & Bluetooth Jammer — Educational Research Project

## 📌 Project Description

This project explores **wireless communication, radio-frequency interference, and network security** using an ESP32 microcontroller and an nRF24L01 wireless transceiver module. It is intended for educational purposes, helping students understand wireless communication concepts, SPI communication, microcontroller interfaces, and the importance of reliable and secure wireless networks.

The project uses the Arduino IDE for development and is designed as a learning resource for electronics, embedded systems, and wireless technology.

> **Disclaimer:** This project is for educational and research purposes only. Any practical experiments must be conducted in a controlled environment with proper authorization. Deliberately interfering with Wi-Fi, Bluetooth, or other wireless communications may be illegal and can disrupt nearby devices and networks. This repository does not endorse unauthorized signal interference.

> ### DOWNLOAD THE FILE OR COPY & PASTE THE CODE IN ARDUINO IDE 

## 🛠️ Required Software

- **Arduino IDE** — for writing, compiling, and uploading firmware to the ESP32.
- **ESP32 Board Package** — provides ESP32 support in the Arduino IDE.
- **RF24 Library** — for communicating with the nRF24L01 module in supported educational experiments.

## 🔧 Required Hardware

- 1 × ESP32 development board
- 1 × nRF24L01 wireless transceiver module
- 7 × jumper wires, as a listed project supply (the actual number and type of wires may vary depending on the wiring configuration)

**Hardware note:** The nRF24L01 communicates over SPI and operates in the 2.4 GHz ISM band. It is not a native Wi-Fi or Bluetooth transceiver and cannot, by itself, implement general-purpose Wi-Fi or Bluetooth jamming.

## 🔌 SPI Pin Reference

The following pin assignments are reference configurations for connecting compatible SPI peripherals to an ESP32. Select the configuration that matches your firmware and hardware.

### HSPI Configuration

| Signal | ESP32 GPIO |
|---|---:|
| SCK | GPIO 14 |
| MISO | GPIO 12 |
| MOSI | GPIO 13 |
| CS / CSN | GPIO 15 |
| CE | GPIO 16 |

### VSPI Configuration

| Signal | ESP32 GPIO |
|---|---:|
| SCK | GPIO 18 |
| MISO | GPIO 19 |
| MOSI | GPIO 23 |
| CS / CSN | GPIO 21 |
| CE | GPIO 22 |

**Important wiring notes:**
- SCK, MISO, MOSI, and CSN are SPI-related connections; CE is a separate control pin for the nRF24L01.
- Verify the selected SPI interface and pin assignments in your firmware before connecting the module.
- Check the exact nRF24L01 module's voltage requirements. The radio module's supply is typically **3.3 V**, not 5 V. Do not connect its power pin directly to 5 V.
- Provide a stable 3.3 V supply and suitable decoupling according to the module's requirements.

## 🎯 Learning Objectives

- Understand wireless communication and radio-frequency concepts.
- Learn ESP32 GPIO configuration and SPI communication.
- Practice embedded programming using the Arduino IDE.
- Explore wireless reliability, interference, and network security.
- Apply responsible and legal practices when conducting electronics experiments.

## ⚖️ Responsible Use

This repository is intended for classroom learning, authorized laboratory testing, and research into wireless communication. Do not use the hardware or software to disrupt public networks, interfere with other people's devices, or impair emergency and essential communications. Follow applicable radio regulations and institutional safety requirements.

## 📚 Technologies

`C++` · `Arduino IDE` · `ESP32` · `nRF24L01` · `SPI` · `Embedded Systems` · `Wireless Communication`

---

**Educational project:** Built to support learning in electronics, embedded systems, and wireless communication security.
