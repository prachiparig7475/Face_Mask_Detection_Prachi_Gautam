# 😷 Face_Mask_Detection_Prachi_Gautam

A real-time face mask detection system built with Python and computer vision. It detects faces from a webcam feed or a web interface and classifies whether each person is wearing a mask or not wearing a mask, with live analytics.

✨ Features
🎥 Live detection using your webcam (detect_live.py)
🌐 Web interface to run detection from the browser (app.py + index.html)
📊 Analytics on detection results such as mask vs. no-mask counts (analytics.py)
⚙️ Central configuration for paths, thresholds and settings (config.py)
⚡ Fast, real-time predictions with a confidence score on every face

---

📁 Project Structure
Face_Mask_Detection_Prachi_Gautam/
│
├── app.py            # Web application (backend server)
├── index.html        # Frontend page for the web app
├── detect_live.py    # Real-time detection using webcam
├── analytics.py      # Detection statistics and analytics
├── config.py         # Configuration (model path, thresholds, etc.)
└── README.md         # Project documentation

---

🛠️ Tech Stack
Language: Python 3.8+
Computer Vision: OpenCV
Deep Learning: TensorFlow / Keras
Web Framework: Flask
Frontend: HTML, CSS, JavaScript
Libraries: NumPy, Pandas

---

🚀 Installation
Clone the repository
bash
   git clone https://github.com/prachiparig7475/Face_Mask_Detection_Prachi_Gautam.git
   cd Face_Mask_Detection_Prachi_Gautam
Create a virtual environment (recommended)
bash
   python -m venv venv
   venv\Scripts\activate        # Windows
   source venv/bin/activate     # macOS / Linux
Install dependencies
bash
   pip install opencv-python tensorflow flask numpy pandas
▶️ Usage

---

1. Live detection with webcam
bash
python detect_live.py

Press q to quit the webcam window.

---

2. Web application
bash
python app.py

Then open your browser and go to: http://127.0.0.1:5000

---

3. Analytics
bash
python analytics.py
⚙️ Configuration

You can change settings such as the model path, confidence threshold and camera index in config.py.

🔍 How It Works
The webcam frame (or uploaded image) is captured.
Faces are detected in the frame.
Each face is pre-processed (resized and normalized) and passed to the trained model.
The model predicts Mask or No Mask with a confidence score.
The result is drawn on the frame with a coloured box (🟢 mask / 🔴 no mask) and logged for analytics.

---

🔮 Future Improvements
Support for multiple faces with improved accuracy in low light
Alert/notification system for people without masks
Deployment on cloud platforms
Dashboard with detailed analytics and reports
👩‍💻 Author

Prachi Gautam GitHub: @prachiparig7475
