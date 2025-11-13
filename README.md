# Graduate Admission Prediction using Neural Networks

This project builds a simple Artificial Neural Network (ANN) to predict the **Chance of Admission** for graduate applicants based on factors such as GRE, TOEFL, university rating, SOP, LOR, CGPA, and research experience.

The dataset used is **Admission_Predict_Ver1.1.csv**.

---

## 📊 Project Overview

The goal of this project is to:

- Load and understand the dataset  
- Preprocess the features  
- Scale numerical inputs  
- Build a regression Neural Network model using Keras  
- Evaluate model performance using R² score  
- Visualize training and validation loss  

This is a beginner-friendly end-to-end machine learning workflow.

---

## 🧠 Dataset Information

The dataset contains the following features:

- **GRE Score**
- **TOEFL Score**
- **University Rating**
- **SOP Strength**
- **LOR Strength**
- **CGPA**
- **Research (0/1)**  
- **Chance of Admit (Target variable)**

The column *Serial No.* was removed as it is not useful for modeling.

---

## 🛠️ Technologies Used

- **Python**
- **Pandas**
- **NumPy**
- **Scikit-Learn**
- **TensorFlow / Keras**
- **Matplotlib**

---

## 🔧 Steps Performed

### 1. Load Dataset  
Used Pandas to read and inspect data.

### 2. Data Cleaning  
- Removed unnecessary column  
- Checked for duplicates  
- Verified dataset structure

### 3. Feature Scaling  
Used **MinMaxScaler** to scale the input features.

### 4. Train-Test Split  
Split the dataset into training and testing sets using `train_test_split`.

### 5. Neural Network Model  
A simple ANN using Keras:

- Input layer: 7 features  
- Hidden Layer 1: Dense(7, ReLU)  
- Hidden Layer 2: Dense(7, ReLU)  
- Output Layer: Dense(1, Linear)  

Loss: Mean Squared Error  
Optimizer: Adam  

### 6. Model Training  
Trained for 100 epochs with validation split of 20%.

### 7. Evaluation  
Used **R² score** to evaluate model performance on the test set.

### 8. Visualization  
Plotted training and validation loss curves using Matplotlib.

---

## 📈 Results

- **R² Score:** (Displayed in notebook after training)
- The model captures trends well but may be improved using deeper networks or different algorithms.

---

## 📂 How to Run

1. Clone the repository:  
   ```bash
   git clone <your-repo-url>
