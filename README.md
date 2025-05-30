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
![Image](https://github.com/user-attachments/assets/d356e4be-6bc2-49e8-984c-7fd68ba32df9)
![Image](https://github.com/user-attachments/assets/f499ee98-e032-48b7-991e-624b93159f8d)
![Image](https://github.com/user-attachments/assets/9665057b-8991-431a-b14a-f18087e0e77e)
![Image](https://github.com/user-attachments/assets/fb299d81-61f4-40a9-bd35-a9ac7bed0d81)
![Image](https://github.com/user-attachments/assets/bb600041-69a8-4b0c-9b28-a8262c64dbcd)
![Image](https://github.com/user-attachments/assets/7018920a-8cbf-4bc7-9c2d-cc65a5e5f78e)


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


