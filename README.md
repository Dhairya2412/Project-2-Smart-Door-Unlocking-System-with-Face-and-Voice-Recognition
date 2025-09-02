🛡 Enhanced BioAuth System

An AI-powered biometric authentication system combining facial recognition, voice authentication, and liveness detection for secure, contactless access control.
Built with Streamlit, OpenCV, Resemblyzer, and dlib, this project provides a modern alternative to conventional door-locking systems like keys, PINs, and RFID cards.

🚀 Features

🎙 Voice Authentication using Resemblyzer
 embeddings

👤 Face Recognition with OpenCV-based embeddings

👀 Liveness Detection using dlib (eye-blink, head, and mouth movement)

🔐 Multi-factor Security Levels:

Standard → Voice OR Face

High → Voice AND Face

Maximum → Face with Active Liveness Verification

📊 Admin Dashboard:

Register/Delete users

Capture face and voice samples

Retrain models on demand

View registered users and stats

📩 Real-time Alerts via logs (extendable to Email/SMS)

🎨 Modern UI with custom CSS for dark theme

🛠 Tech Stack

Frontend & Dashboard: Streamlit

Face Recognition: OpenCV (Haar Cascades + HOG Embeddings)

Voice Authentication: Resemblyzer (Speaker embeddings)

Liveness Detection: dlib (Facial landmarks, blink & movement detection)

Audio Handling: sounddevice, wavio, librosa

Data Handling: numpy, pandas, pickle

📂 Project Structure
📦 Enhanced-BioAuth
 ┣ 📂 face_data/             # Stored face images
 ┣ 📂 voice_data/            # Stored voice samples
 ┣ 📜 face_encodings.pkl     # Trained face embeddings
 ┣ 📜 voice_embeddings.pkl   # Trained voice embeddings
 ┣ 📜 app.py                 # Main Streamlit application
 ┣ 📜 requirements.txt       # Dependencies
 ┣ 📜 README.md              # Documentation
 ┗ 📜 shape_predictor_68_face_landmarks.dat  # dlib model (download separately)

⚙️ Installation
1. Clone the repo
git clone https://github.com/yourusername/enhanced-bioauth.git
cd enhanced-bioauth

2. Install dependencies
pip install -r requirements.txt

3. Download dlib face landmark model

Download shape_predictor_68_face_landmarks.dat from:
👉 dlib model download link

Place it in the project root directory.

▶️ Usage

Run the Streamlit app:

streamlit run app.py

🖥 Modes

Authentication Mode → Secure login with face/voice biometrics

Admin Panel (password: Admin@123) → Register, delete, and manage users

🔐 Security Levels

Standard: Authenticate with Face OR Voice

High: Authenticate with Face AND Voice

Maximum: Authenticate with Face + Active Liveness

📌 Future Improvements

Add email/SMS alerts for failed login attempts

Improve face embedding model (e.g., FaceNet, DeepFace)

Support mobile-based access (via Streamlit Cloud or API)

Hardware integration (smart locks / IoT relays)

📝 License

This project is licensed under the MIT License – free to use and modify.

✨ With Enhanced BioAuth, you get a foolproof, AI-powered, and user-friendly access control system for homes, offices, and restricted areas.
