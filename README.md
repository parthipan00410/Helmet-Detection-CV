# 🪖 Helmet Detection – Workplace Safety Monitoring (Computer Vision)

## 📌 Problem Statement  
Workplace safety in hazardous environments like **construction sites** and **industrial plants** is crucial to prevent accidents and injuries. One of the most important safety measures is ensuring workers wear **safety helmets**, which protect against head injuries from falling objects and machinery.  

Manual monitoring of helmet compliance is:  
- Error-prone  
- Labor-intensive  
- Hard to scale in large operations  

This project develops an **automated helmet detection system** using Computer Vision and Deep Learning to improve safety enforcement and reduce risks.  

---

## 🎯 Objective  
The goal is to build an **image classification model** that detects whether a worker is:  
- ✅ **With Helmet** (wearing a safety helmet)  
- ❌ **Without Helmet** (not wearing a safety helmet)  

This model will serve as the foundation for a **real-time monitoring system** to ensure compliance with workplace safety regulations.  

---

## 📂 Data Description  
The dataset consists of **631 labeled images**:  
- **311 images** → Workers **with helmets**  
- **320 images** → Workers **without helmets**  

Characteristics:  
- Collected from **construction sites, factories, and industrial settings**  
- Includes variations in **lighting, angles, and postures**  
- Workers engaged in different activities (standing, moving, using tools)  

---

## 🛠️ Tech Stack  
- **Language:** Python  
- **Libraries:** TensorFlow, Keras, NumPy, Pandas, Matplotlib, Seaborn, scikit-learn  
- **Techniques:** Image Preprocessing, Data Augmentation, CNNs, Transfer Learning (VGG16)  
- **Environment:** Google Colab  

---

## 🚀 Approach  
1. **Data Preparation**  
   - Images resized to `(200, 200, 3)`  
   - Labels encoded (`With Helmet = 1`, `Without Helmet = 0`)  
   - Train-test split  

2. **Exploratory Data Analysis (EDA)**  
   - Visualized random samples  
   - Checked class distribution  
   - Analyzed lighting/angle variations  

3. **Model Development**  
   - **CNN Model** (built from scratch)  
   - **Transfer Learning with VGG16** for improved accuracy  
   - Dropout & Batch Normalization for regularization  

4. **Evaluation Metrics**  
   - Accuracy  
   - Precision  
   - Recall  
   - F1-score  
   - Confusion Matrix  

---

## 📊 Results  
- **CNN Model Accuracy:** ~0.99%  
- **VGG16 Transfer Learning Accuracy:** ~100%  
- Clear improvement using **transfer learning** with pre-trained weights.  

---

## 📌 Key Learnings  
- Automated compliance monitoring reduces **human error** in safety enforcement.  
- Transfer learning boosts performance on small datasets.  
- A deployable model can integrate into **CCTV or real-time monitoring systems**.  
