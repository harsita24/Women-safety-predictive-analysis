WOMEN’S SAFETY PREDICTIVE ANALYTICS
===================================

A smart, AI-powered, voice-activated emergency response system and crime prediction dashboard designed to enhance the safety of women using real-time machine learning, speech recognition, and data visualization.

Overview
--------

This project integrates crime type prediction and crime rate estimation with a voice-triggered alert mechanism. It uses machine learning models to forecast criminal activity and allows users to issue emergency alerts hands-free via voice commands.

Features
--------

- Voice-Activated Emergency Alerts
- Real-Time Crime Type Prediction (Random Forest Classifier)
- Crime Rate Estimation (Random Forest Regressor)
- Interactive Crime Analytics Dashboard
- Risk Zone Mapping with Leaflet.js
- SMS Notification via Twilio
- Real-Time API Integration using Django 

Tech Stack
----------

Backend:
- Python, Django (REST Framework)
- Scikit-learn, Pandas, SpeechRecognition
- Twilio API for SMS alerts
- Joblib for ML model deployment

Frontend:
- React.js
- Chart.js for visualizations
- Leaflet.js for maps
- Web Speech API for browser voice input

Machine Learning Models
------------------------

1. Random Forest Classifier:
   - Predicts crime types like assault, theft, abuse.
   - Uses location, time, and premise data.

2. Random Forest Regressor:
   - Estimates crime rate in a location.
   - Outputs risk level: Low / Medium / High

Evaluation Metrics
------------------

| Metric        | Classifier | Regressor |
|---------------|------------|-----------|
| Accuracy      | 85–90%     | —         |
| Precision     | 82–88%     | —         |
| Recall        | 80–86%     | —         |
| F1-Score      | 81–87%     | —         |
| MAE (Error)   | —          | 5–10      |
| MSE (Error)   | —          | 30–50     |

Setup Instructions
------------------

Prerequisites:
- Python 3.9+
- Node.js 14+
- Virtualenv
- Twilio account (for SMS)

Clone and Run:

```bash
git clone https://github.com/<your-username>/women-safety-analytics.git
cd women-safety-analytics

Backend setup
cd backend
python -m venv venv
source venv/bin/activate    # or venv\Scripts\activate on Windows
pip install -r requirements.txt
python manage.py runserver

Frontend setup
cd ../frontend
npm install
npm start

Voice Activation Setup
Ensure microphone access is enabled. The system listens for “help” or “danger” and automatically sends emergency alerts and starts recording.

Experimentation & Results
Emergency voice command triggers audio recording and SMS alert.
Dashboard displays crime prediction results.
Risk map shows location-based threat levels.

Results



![WhatsApp Image 2025-06-11 at 2 13 25 PM (1)](https://github.com/user-attachments/assets/977d9b74-f434-4fc7-9f46-d1fe2f80de2d)
![WhatsApp Image 2025-06-11 at 2 13 26 PM](https://github.com/user-attachments/assets/657115ec-6432-4fa3-b75a-9f132f4efe93)
![WhatsApp Image 2025-06-11 at 2 13 26 PM (1)](https://github.com/user-attachments/assets/589bb3ae-f50b-4348-af6f-5972d8818742)
![WhatsApp Image 2025-06-11 at 2 13 26 PM (1)](https://github.com/user-attachments/assets/e70ee1e7-1567-4dda-8d04-421f5d58e588)
![WhatsApp Image 2025-06-11 at 2 13 27 PM](https://github.com/user-attachments/assets/85bfb7cb-0d60-4117-9660-f309157e94b0)
![WhatsApp Image 2025-06-11 at 2 13 25 PM](https://github.com/user-attachments/assets/fc58b46e-0b94-479d-8420-3a742f58b288)
