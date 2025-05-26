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

![Output 1](images/sample_output1.png)
![sample_output1 png](https://github.com/user-attachments/assets/dc85b2a5-ebee-418e-8d0b-2b76ac0eb7e3)


![Output 2](images/sample_output2.png)
![sample_output2 png](https://github.com/user-attachments/assets/5c1a26bc-8cad-46e6-abf7-495e1816bfea)

![Output 3](images/sample_output3.png)
![sample_output3 png](https://github.com/user-attachments/assets/b7015ca0-5505-43bc-9c57-955abbecb31f)


![Output 4](images/sample_output4.png)
![sample_output4 png](https://github.com/user-attachments/assets/b6aff1b6-e809-457b-aea6-e7cfa9d3e549)


![Output 5](images/sample_output5.png)
![sample_output5 png](https://github.com/user-attachments/assets/08d73e00-a12a-48fb-9609-2d2281dfb965)

Results & Performance
✅ Overall Accuracy: 95.19%

🔁 Adjustments made for letters: E, J, K, T, Z

⚠️ Confusion observed in: A vs E, K vs V

✔️ Success Rate Table
Alphabet	Accuracy (%)
A-Z	Mostly 100%, some 75%


