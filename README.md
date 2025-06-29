# 🔥 Automatic Temperature-Controlled Fan using AT89C51
---
A standalone smart fan controller that adjusts fan speed based on real-time temperature using AT89C51 microcontroller, LM35 sensor, and software-generated PWM. Designed as a compact, cost-effective embedded system — no IoT or Wi-Fi required!

🧪 Built as part of:
22ECL42 – Microprocessor and Microcontroller Lab
Department of ECE, Kongu Engineering College



## 🛠️ Project Overview

This system:

* Monitors room temperature using an LM35 sensor
* Converts analog data to digital via ADC0804
* Uses the 8051 (AT89C51) microcontroller to:

  * Generate PWM for fan speed control
  * Display temperature and fan status on LCD
* Simulates everything in Proteus 8.17



## 🔧 Components Used

| Component               | Purpose                                |
| ----------------------- | -------------------------------------- |
| AT89C51 Microcontroller | Core processing & logic control        |
| LM35 Temperature Sensor | Measures ambient temperature           |
| ADC0804                 | Converts analog sensor data to digital |
| L293D Motor Driver      | Drives 12V DC Fan                      |
| 16x2 LCD Display        | Shows real-time data                   |
| Power Supply (5V & 12V) | System power                           |
| Proteus 8.17 Software   | Circuit simulation & waveform testing  |



## ⚙️ How It Works

| Temperature (°C) | Fan Status | PWM Signal           | RPM Estimate |
| ---------------- | ---------- | -------------------- | ------------ |
| < 25             | OFF        | 0% Duty Cycle        | 0            |
| 25–30            | Medium     | 50% Duty Cycle       | \~494        |
| > 30             | High       | Constant High (100%) | \~988        |

* PWM is generated in software using Timer0 Interrupts
* Fan speed is driven via L293D based on PWM logic
* LCD shows current temperature and fan status in real-time



## 📷 Screenshots

Insert simulation screenshots or waveform plots here:

* [ ] Proteus circuit design
* [ ] PWM waveform (50% and 100% duty cycle)
* [ ] LCD output at various temperatures



## 🧠 Key Learning Areas

* Microcontroller programming (Assembly / Embedded C)
* Timer-based PWM generation
* ADC interfacing with sensors
* LCD control (8-bit parallel)
* Motor control using H-Bridge driver
* Hardware simulation and debugging in Proteus



## 👨‍💻 Team

* Hariprasad M (23ECR068)
* Kishorekumar S (23ECR117)
* Krishnakumar VR (23ECR118)



## 📂 Repo Contents

| File                    | Description                     |
| ----------------------- | ------------------------------- |
| Title MPMC Report.pdf   | Full project documentation      |
| Temp Fan Control.pdsprj | Proteus simulation project      |
| Auto Temp Fan (100%) 11.0592MHZ.txt | Microcontroller source code |
| /screenshots            | Circuit + PWM waveform captures |



## 🚀 How to Run

1. Clone this repo:

   git clone [https://github.com/your-username/auto-fan-controller]([https://github.com/your-username/auto-fan-controller](https://github.com/kishorekumarsamiyappan/Smart-Fan-Controller-Using-AT89C51-Microcontroller.git))

2. Open Temp Fan Control.pdsprj in Proteus 8.17

3. Upload the source code to the AT89C51 emulator

4. Simulate and test across various temperatures



## 🧩 Real-World Use Cases

* Smart room fan controller
* Offline temperature regulation for labs / server racks
* Embedded systems learning project



📌 Feel free to fork this project or open an issue to collaborate!

If this helped you, ⭐ Star the repo and share the love.
