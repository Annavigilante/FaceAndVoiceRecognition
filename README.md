# 🛡️ Face and Voice Biometric Verification System

This project implements a **Real-Time Biometric Authentication System** using a combination of **face recognition** and **voiceprint verification**. It ensures higher security by requiring both visual and vocal confirmation for identity validation.

---

## 📌 Features

- 🎥 **Face Detection and Recognition** using `face_recognition` and `OpenCV`
- 🎙️ **Voice Recording and Matching** using `sounddevice`, `soundfile`, and `librosa`
- 🧠 Combines both face and voice authentication for double-layered security
- 🖥️ Simple **Tkinter-based GUI** for real-time verification and user interaction
- 💾 User enrollment system for adding new users with face and voice data

---

## 🚀 How It Works

1. **User Enrollment**
   - Capture face and record voice for each user
   - Save face encodings and voice MFCC features to disk

2. **Authentication**
   - System captures live face and voice input
   - Compares against stored data to verify identity
   - Grants access if both face and voice match

---

## 🛠️ Technologies Used

| Component        | Library                              |
|------------------|--------------------------------------|
| Face Recognition | `face_recognition`, `OpenCV`         |
| Voice Features   | `sounddevice`, `soundfile`, `librosa`|
| GUI              | `Tkinter`                            |
| ML/NLP Features  | `numpy`, `scikit-learn`              |

---

## 📂 Folder Structure

```
├── FaceAndVoice.ipynb           # Main Jupyter Notebook
├── known_faces/                 # Stores known face encodings
├── known_voices/                # Stores known voice feature files
├── voice_recordings/           # Temporary voice data for live testing
└── README.md                    # Documentation
```

---

## ⚙️ Installation

Make sure you have Python 3.8+ installed.

```bash
pip install face_recognition opencv-python sounddevice soundfile librosa numpy scikit-learn
```

> ⚠️ If you're on macOS and face_recognition fails, install dlib using Homebrew or Conda.

---

## 🧪 How to Run

1. Open the notebook: `FaceAndVoice.ipynb`
2. Run all cells in order
3. Use the GUI to:
   - Register new users (face + voice)
   - Authenticate users in real-time

The system displays **Access Granted** if both face and voice match, otherwise **Access Denied**.

---

## 🎯 Use Cases

- Secure login systems
- Biometric attendance
- Physical access control
- Smart home authentication

---

## 🧠 Future Scope

- Add deep learning for voice matching
- Anti-spoofing mechanisms for better security
- Replace GUI with modern web dashboard
- Cross-platform packaging using PyInstaller
