# 📘 Module 3 – Keras and Deep Learning Libraries  

This module introduces **Keras**, a high-level deep learning API built on TensorFlow, and demonstrates how to build **regression and classification models** with only a few lines of code.  

---

## 🚀 Key Learnings
- **Keras Basics**  
  - High-level API for rapid prototyping.  
  - Two model types: `Sequential` (linear stack) and Functional API (flexible architectures).  
- **Dense Neural Networks**  
  - Hidden layers use **ReLU** to avoid vanishing gradients.  
  - Output layers depend on task:  
    - **Regression** → Linear activation + MSE loss  
    - **Classification** → Softmax activation + Cross-entropy loss  
- **Optimizers & Metrics**  
  - Used **Adam optimizer** (adaptive learning rate).  
  - Metrics: MAE/MSE for regression, Accuracy for classification.  
- **Training Loop**  
  - `.fit()` handles forward pass, backpropagation, and weight updates.  
  - `validation_split` parameter provides built-in validation.  

---

## 🧩 Labs Completed

### 🔹 Regression (Concrete Dataset)
- Predict compressive strength of concrete based on material proportions.  
- Compared models:  
  - **Small net (2×5)** → Validation RMSE ~10 MPa  
  - **Deep net (5×50)** → Validation RMSE ~3–4 MPa  
- Confirmed deeper networks capture richer feature interactions.  

### 🔹 Classification (Car Dataset)
- Task: classify car purchasing decision (`0=bad, 1=acceptable, 2=good, 3=very good`).  
- Preprocessed target with `to_categorical()`.  
- Built classifier with Softmax output + categorical cross-entropy loss.  
- Achieved **>97% validation accuracy**.  
- Predictions return class probabilities (confidence scores).  

---

## 🔗 Connections
- Builds on **Module 2** (backpropagation + activations): Keras now abstracts these steps.  
- Prepares for **Module 4** (CNNs & RNNs) using the same workflow with specialized layers.  
- Direct applications to Ahmad’s projects:  
  - **Trackr** → Predict focus scores (regression) or classify focus states (classification).  
  - **NeuroFocus** → Classify mental states into multiple categories.  

---

## 🧠 Reflections
- ✅ Gained confidence in using Keras for both regression & classification.  
- ❓ Still curious about tuning architectures (hidden layers, neurons) and adding regularization (Dropout, L2).  
- 🚀 Plan to apply these methods to real-world datasets like student performance prediction.  
- 💡 Idea: extend the classification model into a **recommender system** with explainable probabilities.  

---

## 📂 Repo Structure
module-3-keras/
│ ├── DL0101EN-3-1-Regression-with-Keras.ipynb
│ ├── DL0101EN-3-2-Classification-with-Keras.ipynb
│ └── classification_model.keras
| ── README.md

yaml
Copy code

---

## 🛠️ Tech Stack
- Python  
- TensorFlow / Keras  
- Pandas, NumPy  
- Jupyter Notebook  

---