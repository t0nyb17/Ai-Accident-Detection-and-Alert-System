# 🚨 Accident Detection System

An AI-powered real-time vehicle accident detection system that leverages computer vision and sensor-based data to notify emergency services immediately upon detecting a crash or anomaly. Designed to reduce emergency response time and save lives.

---

## 📌 Table of Contents

- [Demo](#demo)
- [Features](#features)
- [Architecture](#architecture)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
- [How It Works](#how-it-works)
- [Dataset & Models](#dataset--models)
- [Screenshots](#screenshots)
- [Future Improvements](#future-improvements)
- [Contributors](#contributors)
- [License](#license)

## 📸 Screenshots

### 🧭 Dashboard Overview
<img width="1710" alt="Dashboard Screenshot" src="https://github.com/user-attachments/assets/a1126e13-218a-4217-a24e-1da22e46ef24" />

### 📍 Real-Time Accident Alert
<img width="1710" alt="Accident Alert Screenshot" src="https://github.com/user-attachments/assets/eb5ae1b9-d927-4cfd-bfbb-7009d2faf7f5" />

### 📊 Analytics and Reporting
<img width="1710" alt="Analytics Screenshot" src="https://github.com/user-attachments/assets/6cafaad7-89ab-478f-9ff3-47e86a868b7b" />

### 🔐 Secure Login Page
<img width="1414" alt="Login Screenshot" src="https://github.com/user-attachments/assets/c14bb852-f043-45af-b717-1625029724bc" />


---

## 🚀 Demo

A live demonstration video or demo app link can be added here.

> _"Emergency services, automated. Fast, reliable, and intelligent."_  

---

## ✅ Features

- 🔍 Real-time accident detection using YOLOv8.
- 📡 Automatic alert generation and GPS tracking.
- 🧠 ML-based decision system for anomaly detection.
- 📷 CCTV camera & sensor data integration.
- 📧 Email/SMS notifications to emergency contacts.
- 📊 Dashboard for analytics & incident logs (if available).

---

## 🧱 Architecture

```plaintext
Vehicle/CCTV Footage → YOLOv8 Model → Crash Detection Logic
                                 ↓
               Alert System (Email/SMS/API)
                                 ↓
              Emergency Services & User Notification
```

---

## 🛠️ Tech Stack

**Frontend:**
- HTML/CSS/TS/TSX

**Backend:**
- Python (FastAPI / Flask)
- Logistic Regression for Accident or No Accident
- OpenCV for video stream processing
- PyTorch & YOLOv8 for object detection
- SMTP / Twilio (for email/SMS alerts)

**Models:**
- `yolov8.pt`
- Custom-trained `best.pt` model on accident datasets

---

## 🧪 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/umakantchauhan/Accident-Detection-System.git
   cd Accident-Detection-System
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Download YOLOv8 Weights**
   - Place your `best.pt` and `yolov8.pt` files inside `backend/models/`

4. **Run the backend server**
   ```bash
   cd backend
   python app.py
   ```

5. **Frontend (Optional)**
   - Open `index.html` in your browser (if frontend exists)

---

## ⚙️ How It Works

1. System continuously monitors video feed from vehicle or traffic cameras.
2. YOLOv8 model detects accident scenarios (e.g., collisions, vehicle flips).
3. Upon detection, system triggers:
   - Location fetch (via GPS or manual input)
   - Alert dispatch to emergency contact via email or SMS
4. Logs the incident for future analysis.

---

## 📁 Dataset & Models

- **YOLOv8 Model:** Pretrained + fine-tuned on accident datasets
- **Data Source:** Real-world dashcam footage, accident datasets
- Models are stored in `backend/models/`


---

## 🚧 Future Improvements

- Add mobile app integration.
- Enhance detection accuracy with multi-sensor fusion.
- Implement cloud storage for historical logs.
- Use Twilio or Firebase for real-time alerts.
- Real-time dashboard with geolocation analytics.

---

## 👨‍💻 Contributors
- [Shaan Aigal](https://github.com/shaanaigal)
- [Tanmay Bangar(ME)](https://github.com/t0nyb17)
- [Umakant Chauhan](https://github.com/umakantchauhan)

_Contributions, suggestions, and forks are welcome!_

---


> ⚠️ **Disclaimer:** This system is a prototype and should not be solely relied upon for real-time critical accident detection without thorough validation and hardware calibration.
