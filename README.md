# 🗑️ Smart Garbage Classifier (Recycle vs Non-Recycle)

A full-stack ML-powered web app that identifies garbage types across 12 categories using a fine-tuned MobileNetV2 model.

## 🔧 Built Using

- **FastAPI** for backend logic and template rendering  
- **TensorFlow/Keras** for training the classification model  
- **Google OAuth 2.0** for secure user authentication  
- **SQLite with SQLModel** to manage user tokens  
- **OpenWeatherMap API** to show live Air Quality Index (AQI)

---

## 🌟 Key Features

- ✅ Upload an image and receive an instant garbage classification  
- ✅ Secure login via Google OAuth  
- ✅ Each user starts with **1000 tokens**, with **3 tokens used per prediction**  
- ✅ Display of prediction results alongside token balance  
- ✅ Real-time AQI display integrated into the UI  
- ✅ Fully responsive frontend using Jinja2 and HTML/CSS  

---

## 🔐 Google OAuth Integration

1. Visit [Google Cloud Console](https://console.cloud.google.com/apis/credentials)
2. Create new OAuth 2.0 credentials:
   - **Application Type**: Web Application  
   - **Authorized Redirect URI**: `http://localhost:8000/auth`

---

## 🧠 Model Overview

The model was trained on **Google Colab** using:

- ✅ **MobileNetV2** with ImageNet pre-trained weights  
- ✅ Data augmentation: rotation, zoom, and more  
- ✅ Dataset: [Garbage Classification Dataset](https://www.kaggle.com/datasets/mostafaabla/garbage-classification) via KaggleHub  

The final model is saved as `garbage_classifier.h5` in the `/model` folder.

### Supported Classes:
shoes
trash
white glass

### Trained_Model_Link:
https://colab.research.google.com/drive/1bWcOI0bAtcl-RNhpHCTmChenqAeX9mR4?usp=sharing
