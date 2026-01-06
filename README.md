# 🍎 Fruit Classification: Transfer Learning & Fine-Tuning 🍌
## 📌 Overview
This project implements a robust Image Classification pipeline to identify various fruit species using the Fruits-360 dataset. It demonstrates a two-stage training approach: first utilizing Transfer Learning with a pre-trained VGG16 model, followed by Fine-Tuning specific layers to achieve high accuracy.

## 🚀 Key Features
#### 🔄 Transfer Learning:
Leverages VGG16 (pre-trained on ImageNet) to extract powerful features from fruit images.

#### 🎛️ Fine-Tuning Strategy:
Implements a sophisticated workflow that first trains the classifier head, then unfreezes the top 5 layers of VGG16 for precision tuning with a lower learning rate.

#### 🖼️ Data Augmentation: 
Uses ImageDataGenerator for rotation, shifting, shearing, and zooming to prevent overfitting.

#### ⚡ Performance Optimization:
Utilizes Mixed Precision (mixed_float16) for faster training and memory efficiency.

#### 🛑 Advanced Callbacks: 
Integrates ReduceLROnPlateau and EarlyStopping to optimize convergence and prevent wasted epochs.

##### 🛠️ Tech Stack :
      🐍 Python
      
      🧠 TensorFlow & Keras
      
      📉 Matplotlib (Performance Visualization)
      
      🔢 NumPy
      
      ☁️ Wget & Zipfile (Automated Data Retrieval)

## 📂 Dataset
The project automatically downloads the Fruits-360 dataset, organizing it into:

#### Training:
With heavy data augmentation.

#### Validation:  
For monitoring loss during training.

#### Testing:
For final unbiased evaluation.
