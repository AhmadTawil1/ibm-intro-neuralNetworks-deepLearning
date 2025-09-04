# Module 4 – Deep Neural Networks, CNNs, RNNs & Transformers  

## 📘 Overview  
This module explores the transition from shallow neural networks to modern deep architectures, focusing on:  
- Differences between shallow and deep NNs  
- Convolutional Neural Networks (CNNs) for vision tasks  
- Recurrent Neural Networks (RNNs) and LSTMs for sequential data  
- Transformers and attention mechanisms for NLP and multimodal AI  

---

## 🧩 Key Concepts  

### 🔹 Shallow vs Deep Neural Networks  
- **Shallow NN** → 1–2 hidden layers, limited feature extraction.  
- **Deep NN** → 3+ hidden layers, learns hierarchical features directly from raw data.  
- Deep learning boom was driven by:  
  - **ReLU activations** (solved vanishing gradients)  
  - **Big data availability**  
  - **GPU acceleration**  

### 🔹 Convolutional Neural Networks (CNNs)  
- Designed for **image data**.  
- Architecture: **convolution → ReLU → pooling → flatten → dense**.  
- Advantages: parameter efficiency, spatial feature extraction, translation invariance.  
- Applications: image classification, object detection, medical imaging.  

### 🔹 Recurrent Neural Networks (RNNs) & LSTMs  
- Capture **temporal dependencies** by looping hidden states.  
- Vanilla RNNs suffer from **vanishing/exploding gradients**.  
- **LSTM** introduces gates (forget, input, output) → solves long-term dependency problem.  
- Applications: text, time-series, handwriting, speech recognition.  

### 🔹 Transformers  
- Core innovation: **attention mechanism**.  
- **Self-attention** → queries, keys, values compute relevance across tokens.  
- **Cross-attention** → links different modalities (e.g., text → image).  
- Benefits: parallelization, long-range dependency modeling.  
- Limitations: data-hungry, inherits training biases.  
- Applications: machine translation, summarization, ChatGPT, DALL·E, Stable Diffusion.  

---

## 💻 Labs Completed  

### 1. Convolutional Neural Networks with Keras  
- Built CNNs with convolutional, pooling, flatten, and dense layers.  
- Applied softmax for multi-class image classification.  
- Learned how CNNs reduce parameters and capture spatial features.  

### 2. Transformers with Keras  
- Implemented transformer layers with self-attention (Q, K, V, attention scores, weighted sums).  
- Explored cross-attention for text-to-image generation.  
- Understood transformer advantages (parallelization, long-range modeling) and limitations (data-hungry, bias).  

---

## 🧠 Key Takeaways  
- CNNs specialize in **vision tasks**.  
- RNNs/LSTMs specialize in **sequence/time-series tasks**.  
- Transformers are now the **state-of-the-art** in NLP and generative AI.  
- Deep learning progress is powered by **better architectures, more data, and stronger hardware**.  
