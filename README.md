# 🚦 Traffic Sign Recognition  

A deep learning project to classify traffic signs using the **German Traffic Sign Recognition Benchmark (GTSRB)** dataset.  
This project demonstrates data preprocessing, model training, hyperparameter tuning, and evaluation of a **Convolutional Neural Network (CNN)** built with TensorFlow/Keras.  

---

## 🚀 Features  
- Load and preprocess GTSRB dataset  
- Data Augmentation (rotation, scaling, flipping)  
- CNN architecture for traffic sign classification  
- Hyperparameter Tuning for optimization  
- Visualization of training accuracy and loss  
- Test on single images for prediction  

---

## 📊 Dataset  
**GTSRB – German Traffic Sign Recognition Benchmark**  
- 50,000+ images of traffic signs  
- 43 different traffic sign classes  
- Images of varying sizes (resized to 32x32)  

---

## ⚙️ Getting Started  

### ✅ Prerequisites  
- Python 3.7+  
- TensorFlow / Keras  
- NumPy, Pandas, Matplotlib  
- scikit-learn  

# 🧠 Model Architecture  

Input Image (32x32x3)  
        ↓  
Conv2D (32 filters, 3x3) → ReLU → MaxPooling2D (2x2)  
        ↓  
Conv2D (64 filters, 3x3) → ReLU → MaxPooling2D (2x2)  
        ↓  
Conv2D (128 filters, 3x3) → ReLU → MaxPooling2D (2x2)  
        ↓  
Flatten  
        ↓  
Dense (128) → ReLU → Dropout (0.5)  
        ↓  
Dense (64) → ReLU  
        ↓  
Dense (43) → Softmax  

---

# 🔍 Example Prediction  

**Input Image:** 🛑 (Stop Sign)  

- **Predicted Class:** `Stop` ✅  
- **Confidence:** 99.2%  

git clone https://github.com/your-username/traffic-sign-recognition.git
cd traffic-sign-recognition
