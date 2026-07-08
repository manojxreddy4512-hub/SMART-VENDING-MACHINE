# SMART-VENDING-MACHINE
Developed an IoT-based Smart Vending Machine using ESP32, Firebase, and UPI payments. Built a web interface for product selection and cashless checkout. The ESP32 monitored Firebase in real time and automatically dispensed the selected item using servo motors after payment confirmation.

## Overview

The Smart Vending Machine is an IoT-based automated vending system that dispenses products only after successful digital payment. The project integrates a web application, Firebase Realtime Database, and an ESP32 microcontroller to provide a cashless, real-time vending experience. Users select products through a web interface, complete payment using UPI, and receive the selected item automatically after payment confirmation. :contentReference[oaicite:0]{index=0}

## Features

- Cashless UPI payment integration
- Firebase Realtime Database
- ESP32-based automation
- Automatic product dispensing
- Web-based user interface
- Real-time payment monitoring
- Servo motor controlled vending
- Cloud-connected IoT system

## Hardware Components

- ESP32 Development Board
- SG90 Servo Motors
- L298N Motor Driver
- DC Motor
- Relay Module
- 5V Power Supply
- Jumper Wires
- Breadboard

## Software Requirements

- Arduino IDE
- Firebase Realtime Database
- HTML
- CSS
- JavaScript
- Firebase Hosting
- ArduinoJson Library
- Wi-Fi Library

## Technologies Used

- ESP32
- Firebase Realtime Database
- HTML
- CSS
- JavaScript
- UPI Payment
- REST API
- Arduino C++

## Working

1. The web application loads products from Firebase.
2. The user selects products and adds them to the cart.
3. The total amount is calculated automatically.
4. A UPI payment link or QR code is generated.
5. Payment details are stored in Firebase.
6. After payment, the user clicks "I Have Paid."
7. Firebase updates the payment status to "Completed."
8. ESP32 continuously monitors Firebase.
9. When payment is confirmed, ESP32 activates the corresponding servo motor.
10. The selected product is dispensed.
11. ESP32 updates the payment status to "Dispensed."

## System Architecture

User

↓

HTML Web Interface

↓

Firebase Realtime Database

↓

ESP32

↓

Servo Motor

↓

Product Dispensing

## Hardware Connections

Servo 1 → GPIO 13

Servo 2 → GPIO 12

Servo 3 → GPIO 14

L298N IN1 → GPIO 25

L298N IN2 → GPIO 26

Relay → GPIO 33

## Project Structure

```
Smart-Vending-Machine/
│
├── Arduino_Code/
│   └── vending_machine.ino
│
├── Web/
│   ├── index.html
│   ├── style.css
│   └── script.js
│
├── Images/
│   ├── architecture.png
│   ├── hardware.jpg
│   └── webpage.png
│
├── Firebase/
│   └── database.json
│
├── README.md
└── LICENSE
```

## Installation

Clone the repository.

```
git clone https://github.com/your-username/Smart-Vending-Machine.git
```

Open the Arduino project.

Configure the Wi-Fi credentials.

Configure Firebase URL and API keys.

Upload the code to ESP32.

Deploy the web application to Firebase Hosting.

Open the web application.

Select a product.

Complete the UPI payment.

Click "I Have Paid."

The selected product will be dispensed automatically.

## Results

- Successfully displayed products on the web interface.
- Generated UPI payment links dynamically.
- Stored payment records in Firebase.
- Detected payment completion in real time.
- Automatically dispensed the selected product.
- Updated payment status after dispensing. :contentReference[oaicite:1]{index=1}

## Future Improvements

- Stock monitoring
- QR code payment verification
- Mobile application
- Inventory management
- Multiple vending slots
- AI-based demand prediction
- Receipt generation
- Online admin dashboard

## Authors

T. Manoj Kumar Reddy

T. Sai Ganesh

A. Nikhil

S. K. Adil Suhan

Department of Electronics and Communication Engineering

SRM University-AP

## License

This project is developed for educational and research purposes.
