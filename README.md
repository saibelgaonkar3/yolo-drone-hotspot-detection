# yolo-drone-hotspot-detection
# 🚁 YOLOv5 Projects – Real-Time AI for Drones and Disaster Management

This repository documents my work on real-time object detection using YOLOv5 in drone-based and mobile-based applications. Projects focus on socially impactful use cases like aerial hotspot detection and disaster response.

---

## ✅ Project 1: YOLOv5 Aerial Hotspot Detection (Completed)

**Team Phoenix – Drone Club, MIT-WPU**

1) Trained a custom YOLOv5 model to detect and count visual hotspots in drone-captured aerial imagery.  
2) Classification of shapes: circle, triangle, square  
3) Avoids double-counting shapes that are part of a hotspot  
4) Integrated real-time telemetry + object ID tracking + mock GPS logging

📦 Datasets:  
- [Hotspot Dataset (Google Drive)](https://drive.google.com/drive/folders/1CqV3xo4GNSLW-X3P4zRiQwx5ixkLLGUO?usp=drive_link)  
- [Shape Dataset (Roboflow)](https://universe.roboflow.com/purasuas/classifying-shapes)

### 🔧 Key Details
- **Tools**: YOLOv5, PyTorch, OpenCV, LabelImg  
- **Problem**: Detect hotspots (circle in square), shapes, and prevent overcounting  
- **Pipeline**: Annotation → Training → Evaluation → Real-time inference with ID tracking  
- **Enhancements**: Integrated SORT tracker, telemetry logger, and GPS simulator  
- **Optimization**: Tuned for edge deployment on Jetson Nano

### 📈 Results
- Achieved >85% mAP on test dataset  
- ~25 FPS real-time detection performance  
- Unique object ID tracking to avoid repeated counts  
- Logged timestamp, confidence, label, and location to `hotspot_telemetry_log.csv`

### 📄 Sample Log Output
```
Timestamp           | Object_ID  | Label    | Confidence | Latitude   | Longitude
------------------- | ---------- | -------- | ---------- | ---------- | -----------
2025-07-21 18:40:02 | hotspot_3  | hotspot  | 0.92       | 18.52083   | 73.85701
```

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
- Built using Android Studio

### 🔗 Use Case
Designed for rescue workers and field teams to detect humans and send geo-tagged alerts in real-time without needing cloud inference or heavy hardware.

---

## 🔮 What's Next
- Integrate drone navigation + live detection stream  
- Expand to multi-class detection for damage assessment  
- Collaborate with disaster relief agencies for field trials
