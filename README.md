# 🧠 Synthea – AI Powered Assistive Navigation System

Synthea is an AI-based assistive system designed to help visually impaired individuals navigate safely using computer vision and voice interaction.

It works like a smart companion that detects the surroundings and provides real-time voice guidance.

---

## 🚀 Features

### 🔍 1. Navigation System (Obstacle Detection)

The navigation module is the core part of the system.

It uses **YOLOv8 object detection** to identify objects such as people, chairs, vehicles, etc., from a live camera feed.

Once an object is detected, the system analyzes its position (left, right, or center) and gives voice feedback to the user.

**Example:**
> "Person ahead"  
> "Chair on the -15 degrees"

This helps the user understand their surroundings and avoid obstacles in real time.

---

### 😊 2. Emotion Detection

This module uses the **DeepFace library** to detect emotions from faces captured by the camera.

When a person is detected, the system analyzes their facial expression and classifies it into emotions like:
- Happy  
- Sad  
- Angry  
- Surprised  

The result is then spoken out to the user.

**Example:**
> "Person ahead seems happy"

This feature adds extra awareness about people nearby.

---

### 🎙️ 3. Voice Assistant

Synthea includes a built-in voice assistant that allows hands-free interaction.

The system listens to user commands and performs tasks like:
- Telling the current time  
- Searching on Google  
- Opening YouTube  
- Fetching information from Wikipedia  

It uses **SpeechRecognition** for input and **pyttsx3** for voice output.

**Example:**
> "What is the time?"  
> "Play song on YouTube"

---

### 🚨 4. Emergency Alert System

This feature is designed for safety in critical situations.

When triggered, the system:
- Captures an image using the camera  
- Sends an alert message along with the image  
- Uses **Telegram Bot API** to notify a predefined contact  

This ensures that help can be reached quickly in emergencies.

---

## 🧰 Tech Stack

- **Python**
- **OpenCV**
- **YOLOv8**
- **DeepFace**
- **SpeechRecognition**
- **pyttsx3**
- **Telegram Bot API**

---

## 📌 Conclusion

Synthea aims to make navigation easier and safer for visually impaired individuals by combining AI, computer vision, and voice technology into a single system.
