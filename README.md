 🤟 Sign Language Alphabet Recognition using Machine Learning

This project focuses on recognizing static hand gestures of the American Sign Language (ASL) alphabet using image processing and Convolutional Neural Networks (CNN). The goal is to bridge the communication gap between hearing-impaired and non-impaired individuals through real-time gesture recognition.

---

## 📦 Dataset

The dataset comprises **24,000 images** of 26 alphabets captured using OpenCV through a webcam. It includes data from **two different individuals under varying lighting conditions**, split into:
- `Train` set: 18,000 images
- `Validation/Test` set: 6,000 images
dataset/
├── train/
│ ├── A/
│ ├── B/
│ └── ...
└── val/
├── A/
├── B/
└── ...

📁 Folder Structure:

---

## 🛠 Libraries Used

- `TensorFlow` & `Keras`
- `OpenCV`
- `MediaPipe`
- `NumPy`
- `Matplotlib`


## 🖼️ Model Output Samples
![Image](https://github.com/user-attachments/assets/a4a7d329-70a5-45eb-9da6-b5120f83a7ac)

Install all dependencies:
```bash
pip install tensorflow keras opencv-python mediapipe numpy matplotlib

---

## 🧠 Model Architecture

The CNN is built using Keras and consists of:

- **Input Layer**: 48x48 grayscale images  
- **Conv2D Layers**: 16 filters  
- **MaxPooling2D**  
- **Flatten**  
- **Dense Layer** with ReLU activation  
- **Dropout** (rate: 0.4) to reduce overfitting  
- **Softmax Output Layer**

---

## 📈 Features and Image Preprocessing

- Grayscale Conversion (from BGR)
- Feature Extraction & Scaling to 48x48
- Noise Reduction
- ReLU Activation Function

## Model Output Samples

Below are some example prediction outputs from the model:

Results & Performance
✅ Overall Accuracy: 95.19%

🔁 Adjustments made for letters: E, J, K, T, Z

⚠️ Confusion observed in: A vs E, K vs V

✔️ Success Rate Table
Alphabet	Accuracy (%)
A-Z	Mostly 100%, some 75%


