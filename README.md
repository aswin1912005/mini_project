# ♻️ Smart Waste Classification System Using AI and ESP32

## 📌 Overview

The **Smart Waste Classification System** is an AI-powered waste management project that automatically classifies waste into two categories: **Biodegradable** and **Non-Biodegradable**. It integrates an ESP32 microcontroller, ESP32-CAM, IR sensor, a trained deep learning model, and a servo motor to automate waste detection, classification, and segregation.

A Python Flask server receives images captured by the ESP32-CAM, performs local AI inference, and displays the classification results on a web-based dashboard. The ESP32 controls the sorting mechanism based on the predicted category.

## ⚙️ System Workflow

1. **Waste Detection:** The IR sensor detects the presence of waste.
2. **Camera Trigger:** The ESP32 DevKit V1 directly triggers the ESP32-CAM to capture an image.
3. **Image Transmission:** The ESP32-CAM sends the captured image to the Flask server.
4. **AI Classification:** The trained deep learning model classifies the image as biodegradable or non-biodegradable.
5. **Dashboard Display:** The web dashboard displays the captured image and classification result.
6. **Automatic Segregation:** The ESP32 controls a servo motor to direct the waste into the appropriate compartment.
7. **Bin Monitoring:** Ultrasonic sensors can monitor bin fill levels and support capacity alerts.

## 🛠️ Technologies Used

- **Hardware:** ESP32 DevKit V1, ESP32-CAM, IR sensor, servo motor, ultrasonic sensors
- **Programming:** Python, C++ (Arduino)
- **AI / Deep Learning:** Ultralytics YOLO11 classification model
- **Backend:** Python Flask
- **Frontend:** HTML, CSS, JavaScript
- **Image Processing:** OpenCV
- **Communication:** HTTP

## ✨ Features

- AI-based waste classification
- Automatic image capture and transmission
- Biodegradable and non-biodegradable waste identification
- Servo-based automatic waste segregation
- Web dashboard for displaying images and predictions
- Optional ultrasonic bin-level monitoring
- Local AI inference without requiring a cloud AI API

## 🏗️ Architecture

`IR Sensor → ESP32 DevKit V1 → ESP32-CAM → Flask Server → YOLO Model → Web Dashboard`

The ESP32 DevKit V1 triggers the ESP32-CAM directly. Flask handles image reception and AI classification, while the ESP32 controls the sorting mechanism based on the classification result.

## 🎯 Objective

To develop an intelligent and cost-effective waste management prototype that reduces manual sorting, encourages proper waste segregation, and supports more efficient waste disposal.

## 🚀 Future Enhancements

- Add more waste categories, such as metal, paper, plastic, and glass.
- Integrate IoT-based bin monitoring and notifications.
- Store historical classification results and generate analytics.
- Improve classification accuracy using a larger and more diverse dataset.
- Deploy the dashboard on a remote server for monitoring from anywhere.

## 👨‍💻 Project Status

AI-based waste classification and embedded hardware integration project. Features depend on the implemented hardware and software configuration.

