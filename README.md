# 📱 AI-niform Turnstile Access Control System (SMS Version)

> An integrated IoT and computer vision access control solution designed to regulate school uniform compliance, featuring real-time SMS notifications for unauthorized access or entry logs.

<div align="center">

[![GitHub Release](https://img.shields.io/github/v/release/ichiroyamazaki/AI-niformSMS?style=flat-square&color=blue)](https://github.com/ichiroyamazaki/AI-niformSMS/releases)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](LICENSE)
[![Python Version](https://img.shields.io/badge/python-3.8%2B-blue.svg?style=flat-square)](https://www.python.org/)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg?style=flat-square)](https://github.com/ichiroyamazaki/AI-niformSMS/graphs/commit-activity)

</div>

---

## 🚀 Overview

**AI-niformSMS** is an extension of the AI-niform capstone architecture. It bridges computer vision-based uniform detection with physical hardware actuators (turnstiles) and telecommunications infrastructure. When a student approaches the checkpoint, the system evaluates uniform compliance via object detection models. If compliant, the turnstile unlocks; if non-compliant, entry is restricted, and an automated SMS alert is dispatched to designated administrators or guardians.

---

## 💼 Corporate & Creator Credit

* **Developed by:** [Ichiro Yamazaki](https://github.com/ichiroyamazaki)
* **Organization:** GoForAll Worldwide Corporation

---

## ✨ Features

* **AI-Powered Uniform Detection:** Integrates computer vision models (such as YOLO) to scan and verify proper school attire in real time.
* **Turnstile Hardware Integration:** Controls physical gate mechanisms (relays/solenoids) based on AI inference results.
* **Automated SMS Alerts:** Sends instant text notifications regarding access status, violations, or daily summary logs.
* **Logging & Monitoring:** Tracks entry attempts and compliance statistics for administrative review.

---

## 🛠️ Tech Stack

* **Language:** Python 3.8+
* **Computer Vision:** Ultralytics YOLO / OpenCV
* **Hardware Interfacing:** GPIO / Serial communication for turnstile control
* **Messaging:** GSM Module / SMS Gateway API integration

---

## 📦 Project Structure

```text
AI-niformSMS/
├── core/               # Main application and inference logic
├── hardware/           # Turnstile control and GPIO scripts
├── messaging/          # SMS gateway integration scripts
├── requirements.txt    # Python dependencies
├── .env.example        # Template for environment variables
└── README.md           # Project documentation
⚙️ Installation & Setup
1. Clone the Repository
Bash
git clone [https://github.com/ichiroyamazaki/AI-niformSMS.git](https://github.com/ichiroyamazaki/AI-niformSMS.git)
cd AI-niformSMS
2. Install Dependencies
Bash
pip install -r requirements.txt
3. Configure Environment Variables
Copy .env.example to .env and fill in your required API keys, gateway settings, and hardware pin mappings:

Code snippet
SMS_GATEWAY_API_KEY=your_sms_gateway_key_here
TURNSTILE_GPIO_PIN=17
CAMERA_INDEX=0
4. Run the System
Bash
python main.py
🤝 Contributing
Contributions, bug reports, and feature requests are welcome! Feel free to open an issue or submit a pull request.

📜 License
Distributed under the MIT License. See LICENSE for more information.
