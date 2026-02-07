Chicken Voice Health Classification System
📌 Project Overview

The Chicken Voice Health Classification System is a deep learning-based solution designed to detect the health condition of chickens by analyzing their vocal sounds. The system uses audio signal processing and convolutional neural networks to classify chicken sounds into different health categories.

This project aims to assist poultry farmers and veterinary professionals in early disease detection through automated sound analysis.

🎯 Objectives

Detect chicken health condition using voice signals

Classify chicken audio into:

Healthy

Unhealthy

Noise

Provide visual and probability-based output

Build a deployable web application

🧠 Technologies Used

Python

PyTorch

FastAPI

Streamlit

Librosa (Audio Processing)

Docker (Deployment)

Git & GitHub

📂 Project Structure
chick_voice/
│
├── api_server.py          # FastAPI backend
├── app.py                 # Streamlit UI
├── model.py               # Deep learning model
├── dataset.py             # Dataset loader
├── train.py               # Model training script
├── infer.py               # Model testing script
├── requirements.txt       # Dependencies
├── runtime.txt            # Python version config
├── models/
│     └── chicken_resnet_best.pt

🔬 Model Architecture

The project uses a modified ResNet-18 Convolutional Neural Network for audio classification.

Processing Steps:

Audio input loading

Audio normalization

Mel Spectrogram conversion

CNN feature extraction

Health classification

📊 Output Features

The system provides:

Audio Preview

Mel Spectrogram Visualization

Class Probability Distribution

Health Prediction Result

🚀 How To Run The Project Locally
Step 1 – Clone Repository
git clone https://github.com/YOUR_USERNAME/chick_voice.git
cd chick_voice

Step 2 – Create Virtual Environment
python -m venv venv


Activate environment:

Windows:

venv\Scripts\activate


Linux / Mac:

source venv/bin/activate

Step 3 – Install Dependencies
pip install -r requirements.txt

Step 4 – Run API Server
uvicorn api_server:app --reload

Step 5 – Run Streamlit UI
streamlit run app.py

🌐 API Usage
Endpoint:
POST /predict

Input:

WAV audio file

Output:

Predicted health class

Probability values

🐳 Docker Deployment (Optional)

Build Docker Image:

docker build -t chicken-health .


Run Container:

docker run -p 8000:8000 chicken-health

📈 Future Improvements

Real-time poultry farm monitoring

Mobile application integration

Multi-disease classification

Edge device deployment

Larger dataset training

🤝 Contribution Guidelines

Fork repository

Create feature branch

Commit changes

Submit pull request

📜 License

This project is developed for academic and research purposes.

👨‍💻 Author

Chandra Prakash (CP)
