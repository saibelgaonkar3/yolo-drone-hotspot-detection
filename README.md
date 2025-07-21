# yolo-drone-hotspot-detection
# 🚁 YOLOv5 Projects – Real-Time AI for Drones and Disaster Management

This repository documents my work on real-time object detection using YOLOv5 in drone-based and mobile-based applications. Projects focus on socially impactful use cases like aerial hotspot detection and disaster response.

---

## ✅ Project 1: YOLOv5 Aerial Hotspot Detection (Completed)

**Team Phoenix – Drone Club, MIT-WPU**

1) Trained a custom YOLOv5 model to detect and count visual hotspots in drone-captured aerial imagery.
2) Classification of shapes: circle, triangle, square
hotspot dataset: https://drive.google.com/drive/folders/1CqV3xo4GNSLW-X3P4zRiQwx5ixkLLGUO?usp=drive_link
shapes dataset: https://universe.roboflow.com/purasuas/classifying-shapes


### 🔧 Key Details
- **Tools**: YOLOv5, PyTorch, OpenCV, LabelImg  
- **Problem**: Detect circular hotspots from drone video feed  
- **Pipeline**: Data annotation → model training → evaluation → real-time deployment  
- **Optimization**: Tuned for edge deployment on lightweight devices (Jetson Nano)

### 📈 Results
- Achieved >85% mAP on test dataset  
- ~25 FPS real-time detection performance  
- Successfully deployed on drone-mounted edge devices

---

## 🧭 Project 2: YOLOv5 for Human Detection in Disaster Zones (NIDAR 2025 – Ongoing)

Developing a real-time human detection system for disaster-struck areas using **YOLOv5**, as part of the **NIDAR 2025 AI/ML Challenge**.

### 🎯 Objective
- Detect human survivors from drone or satellite imagery  
- Support emergency response teams during natural disasters

### 🛠️ Tech Stack
- YOLOv5, PyTorch, OpenCV, custom-annotated datasets  
- Training on real disaster data (thermal, aerial)  
- Optimized for low-power devices like Jetson Nano

### 🌍 Impact
Supports faster search and rescue by automating survivor identification in affected areas.

---

## 📱 Project 3: Android-Based Human Detection with GPS + Firebase (Ongoing)

Building a YOLOv5-powered **Android app** that performs on-device object detection and GPS location reporting.

### 🔧 Features
- **YOLOv5s-fp16.tflite** model with custom `labels.txt`  
- **CameraX API** for real-time frame analysis  
- **FusedLocationProviderClient** for precise location  
- Sends detection data + location to **Firebase Realtime Database**
- Used android studio to build app

### 🔗 Use Case
Designed for rescue workers and field teams to detect humans and send geo-tagged alerts in real-time without needing cloud inference or heavy hardware.

---

## 🔮 What's Next
- Integrate drone navigation + live detection stream  
- Expand to multi-class detection for damage assessment  
- Collaborate with disaster relief agencies for field trials

---
