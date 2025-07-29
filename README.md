🛡️ Face and Voice Biometric Verification System
This project implements a Real-Time Biometric Authentication System using a combination of face recognition and voiceprint verification. It ensures higher security by requiring both visual and vocal confirmation for identity validation.
📌 Features
🎥 Face Detection and Recognition using face_recognition and OpenCV
🎙️ Voice Recording and Matching using sounddevice, soundfile, and librosa
🧠 Combines both face and voice authentication for double-layered security
🖥️ Simple Tkinter-based GUI for real-time verification and user interaction
💾 User enrollment system for adding new users with face and voice data
🚀 How It Works
User Enrollment
Capture face and record voice for each user
Save face encodings and voice MFCC features to disk
Authentication
System captures live face and voice input
Compares against stored data to verify identity
Grants access if both face and voice match
🛠️ Technologies Used
Component	Library
Face Recognition	face_recognition, OpenCV
Voice Features	sounddevice, soundfile, librosa
GUI	Tkinter
ML/NLP Features	numpy, sklearn
📂 Folder Structure
├── FaceAndVoice.ipynb           # Main Jupyter Notebook
├── known_faces/                 # Stores known face encodings
├── known_voices/                # Stores known voice feature files
├── voice_recordings/           # Temporary voice data for live testing
└── README.md                    # Documentation
⚙️ Installation
pip install face_recognition opencv-python sounddevice soundfile librosa numpy scikit-learn
⚠️ Make sure you are using Python 3.8 or above with compatible versions of the libraries.
🧪 How to Run
Run the notebook: FaceAndVoice.ipynb
Use the GUI to:
Register new users
Authenticate existing users
System will show Access Granted if both face and voice match, else Access Denied.
🎯 Use Cases
Secure login systems
Biometric attendance
Physical access control systems
Smart home/IoT authentication
🧠 Future Scope
Add model-based speaker recognition (using SVM/Neural Networks)
Enhance spoof detection for security
Replace GUI with a modern web dashboard
Deploy as a cross-platform desktop app using PyInstaller
