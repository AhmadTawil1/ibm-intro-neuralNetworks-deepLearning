# ✈️ Aircraft Damage Classification & Captioning using Pretrained Models

## 📘 Project Overview
Aircraft damage detection is essential for aviation safety and timely maintenance. Traditional manual inspection is time-consuming and prone to human error.  
This project leverages **deep learning** to:
1. **Classify aircraft damage** into two categories: **Dent** and **Crack** using a pretrained **VGG16** model.
2. **Generate captions and summaries** of damage images using a pretrained **BLIP (Bootstrapping Language-Image Pretraining)** Transformer model.

By combining **computer vision** (VGG16) with **vision-language models** (BLIP), this project demonstrates how automation can support aviation safety inspections with both structured outputs (class labels) and natural language explanations.

---

## 🎯 Aim of the Project
- Develop an automated pipeline that:
  - Detects **dent vs crack** from aircraft images.
  - Produces **natural language captions & summaries** describing the damage.
- Showcase integration of **pretrained models** (transfer learning) for real-world safety inspection tasks.

---

## 🛠️ Tech Stack
- **Frameworks:** TensorFlow, Keras, Hugging Face Transformers  
- **Models:** VGG16 (feature extractor), BLIP (captioning & summarization)  
- **Languages:** Python 3  
- **Libraries:** NumPy, Matplotlib, PIL, urllib, tarfile, shutil  

---

## 📂 Dataset
- **Source:** [Roboflow Aircraft Dataset](https://public.roboflow.com) (CC BY 4.0 License)  
- **Classes:**  
  - `dent`  
  - `crack`  
- **Splits:** Training / Validation / Testing  

---

## 🚀 Project Workflow

### Part 1: Classification with VGG16
1. **Dataset Preparation**
   - Train/Validation/Test splits.
   - Data generators with rescaling & preprocessing.
2. **Model Architecture**
   - Pretrained VGG16 (ImageNet weights) as feature extractor.
   - Custom dense layers + dropout for binary classification.
3. **Training**
   - Optimizer: Adam (lr = 0.0001)  
   - Loss: Binary Crossentropy  
   - Metrics: Accuracy
4. **Evaluation**
   - Training & validation accuracy/loss curves.
   - Final test accuracy: **~84%**  
5. **Visualization**
   - Predictions compared against true labels.

### Part 2: Captioning & Summarization with BLIP
1. **BLIP Processor & Model** loaded from Hugging Face (`Salesforce/blip-image-captioning-base`).
2. **Custom Keras Layer** `BlipCaptionSummaryLayer` implemented for text generation.
3. **Helper Function** `generate_text` built to easily switch between **caption** and **summary** tasks.
4. **Results**:
   - **Caption Example:** `this is a picture of a plane`
   - **Summary Example:** `this is a detailed photo showing the engine of a boeing 747`

---

## 📊 Results
- **Classification Accuracy (Test Set):** ~84%  
- **Model Generalization:** Training accuracy improves steadily; validation accuracy stabilizes around ~71%.  
- **Caption & Summary Generation:** Produces human-readable descriptions, though sometimes generic due to dataset/model limitations.  

---

## 🔗 Key Learnings
- Transfer learning with **VGG16** accelerates convergence and improves accuracy on small datasets.
- **Custom Keras layers** allow seamless integration of non-TensorFlow models (e.g., Hugging Face BLIP).
- Combining **classification** and **captioning** bridges the gap between **structured AI outputs** and **human-readable explanations**.

---

## 📌 Future Improvements
- Fine-tune BLIP on **domain-specific aviation data** for more precise captions.  
- Add **object detection** (e.g., bounding boxes) before classification.  
- Deploy the model in a web app for real-time inspection use cases.  

---

## 🏆 Completion
This project was completed as the **Final Project** for the **IBM AI Engineering Professional Certificate (Deep Learning Course)**.

---
