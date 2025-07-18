# AI-Driven Facial Emotion Detection with Music Recommendation and Mental Health Tip

## 📖 Overview

Presents an intelligent wellness system that integrates **AI-powered facial emotion recognition** with **personalized music recommendation** and **mental health tips**. The goal is to enhance emotional well-being by identifying the user's mood through facial expressions and responding with therapeutic content tailored to that mood.

---

## 🚀 Features

- 🧠 **Facial Emotion Detection** using CNN and MediaPipe Face Mesh
- 🎵 **Music Recommendation System** tailored to the user's current emotional state
- 🩺 **Mental Health Tips** generated based on detected mood
- 🧾 **Emotion History Tracking** for user self-awareness over time
- 🔒 **User Authentication** with facial recognition login
- 📊 **Real-Time Analytics** and emotion trend visualization
- 🎮 **GUI Interface** built with Tkinter for easy interaction

---

## 🧰 Tech Stack & Tools

| Technology        | Usage                              |
|------------------|-------------------------------------|
| Python           | Core programming language           |
| TensorFlow & Keras | Deep Learning model (CNN)         |
| OpenCV           | Image processing and face detection |
| MediaPipe        | Facial landmark detection (Face Mesh) |
| Tkinter          | GUI Development                     |
| Pyttsx3          | Text-to-speech for tips             |
| Pygame           | Playing music based on emotion      |

---

## 🛠️ System Architecture

The emotion detection system uses a **multi-CNN pipeline** to analyze facial components:
- CNN-1: Eyebrow + Eye Region
- CNN-2: Eye Detection
- CNN-3: Mouth Region
- Logical operations (AND/OR) consolidate features before final expression detection via CNN-4.

MediaPipe extracts landmarks → Features mapped → Processed by CNN → Emotion classified → Output personalized recommendation (music + tip).

![Architecture Diagram Placeholder]

---

## 📂 Folder Structure
AI-Emotion-Music-Recommendation/
│
├── dataset/ # Training datasets (FER-2013 or custom)
├── models/ # Trained CNN models
├── music/ # Music files categorized by emotion
├── src/ # Core application logic
│ ├── emotion_detect.py # CNN model + prediction pipeline
│ ├── music_player.py # Music recommendation logic
│ ├── health_tips.py # Tip generation module
│ ├── gui.py # Tkinter GUI interface
│ └── login_auth.py # User authentication logic
│
├── logs/ # User emotion history logs
├── requirements.txt # Required Python packages
├── README.md # Project documentation
└── main.py # Entry point of the application



---

## 📸 Input & Output Flow

1. **User Login** ➝ Secure authentication
2. **Image Upload** ➝ Captures or selects face image
3. **Emotion Detection** ➝ Model predicts (Happy, Sad, Angry, etc.)
4. **Output**:
   - 🎵 Emotion-aligned music played
   - 🧘‍♂️ Health tip shown via speech/text
   - 📊 Emotion trend tracked & saved

---

## 🧪 Results

- **Accuracy**: ~75% emotion detection accuracy on varied datasets
- **Real-time Feedback**: Emotion → Instant music + tip
- **User Satisfaction**: Interactive and personalized response boosts user engagement
- **Emotion Trends**: Graphs generated over time for emotional awareness

---

## ✅ Requirements

- Python 3.8+
- TensorFlow
- OpenCV
- Keras
- MediaPipe
- Tkinter
- Pygame
- Pyttsx3

Install all dependencies using:

```bash
pip install -r requirements.txt


▶️ How to Run the Project
Clone the repo:

git clone https://github.com/yourusername/AI-Emotion-Music-Recommendation.git
cd AI-Emotion-Music-Recommendation
Install dependencies:
pip install -r requirements.txt
Run the main file:


python main.py
📈 Future Scope
Real-time webcam-based emotion detection
Integration with wearable sensors (heart rate, etc.)
Expand dataset for multilingual emotion cues
Mobile app version using Flutter/Kivy
Enhanced privacy features and data anonymization

🔒 Ethical Considerations
Respect user privacy and ensure data is processed locally.
No image or emotion data is uploaded/stored on external servers.
Designed with transparency and user consent in mind.

