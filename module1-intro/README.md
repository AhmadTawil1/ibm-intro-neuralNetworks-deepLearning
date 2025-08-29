# Module 1 – Introduction to Deep Learning & Neural Networks with Keras

## 📘 Overview
This module introduces the **foundations of deep learning** and **artificial neural networks (ANNs)**.  
It covers the basic building blocks (neurons, layers, activations), explains forward propagation, and demonstrates how deep learning models extend traditional machine learning by capturing nonlinear relationships.

---

## 🎯 Learning Objectives
By the end of this module, I can:
- Describe recent **applications of deep learning** (color restoration, speech enactment, handwriting generation, translation, self-driving, etc.).
- Explain the **mathematical formulation of neural networks** (weights, biases, linear combination).
- Differentiate between **input, hidden, and output layers** in ANNs.
- Understand and compute **forward propagation** step by step.
- Explain the role of **activation functions** and why they make neural networks nonlinear (vs. linear regression).

---

## 🧪 Lab Completed – *Artificial Neural Networks.ipynb*
In this lab, I:
1. **Initialized weights & biases** using NumPy.
2. **Defined input values** and computed weighted sums for hidden neurons.
3. Applied the **sigmoid activation function** to introduce non-linearity.
4. Performed **forward propagation** through a small network:
   - Input layer → Hidden layer → Output layer.
5. Generated the **final prediction** of the ANN for given inputs.

**Key Insight:**  
Forward propagation = Linear regression + activation functions, stacked layer by layer.  
Without activations, ANNs collapse to linear models.

---

## 📂 Repository Structure (for this module)
├── Artificial Neural Networks.ipynb # Hands-on lab notebook
├── README.md # This file

yaml
Copy code

---

## 📈 Skills Gained
- Mathematical understanding of **ANNs**.
- Hands-on with **NumPy** for simulating forward propagation.
- Ability to **trace weights, biases, activations, and outputs** step by step.
- Recognized why **activation functions are essential** for deep learning.

---

## 🔗 Connection to Next Modules
- Next up: **Backpropagation & Training** — learning how weights and biases are optimized automatically.
- Builds the foundation for **Keras implementation** of deep learning models (regression & classification).
- Paves the way for advanced architectures (CNNs, RNNs, Transformers).

---

## 🧠 Reflection
- ✅ **What I mastered:** The mechanics of forward propagation and how activations add nonlinearity.  
- ❓ **What I’m curious about:** How backpropagation actually adjusts weights to minimize error.  
- 🚀 **Where I’ll apply this:** Building small ANNs in Keras for classification tasks before moving into CNNs and RNNs.  
- 💡 **Idea:** Visualize forward propagation with an interactive tool (sliders for weights/biases) to strengthen intuition.