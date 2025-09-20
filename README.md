# 🦷 Teeth Classification & Disease Detection  

An **AI-powered computer vision system** for automatic teeth classification and dental disease detection using **deep learning**.  
This project leverages preprocessing, visualization, transfer learning, and evaluation pipelines to classify dental images into **7 categories**, supporting dentists with **AI-assisted diagnosis** and improved treatment planning.  

---

## 📖 Overview  

The system classifies dental images into the following categories:  
- **CaS** – Cavity Stage  
- **CoS** – Composite Stage  
- **Gum** – Gum Issues  
- **MC** – Missing Crown  
- **OC** – Oral Cavity  
- **OLP** – Oral Lichen Planus  
- **OT** – Other Teeth Conditions  

✅ This project contributes to advancing **AI-driven dental healthcare**, enhancing **diagnostic accuracy** and **clinical decision-making**.  

---

## 🎯 Objectives  

- **Preprocessing**  
  - Normalize & resize images (256×256).  
  - Apply data augmentation (flips, brightness, contrast, saturation).  

- **Visualization**  
  - Display representative samples per class.  
  - Analyze dataset balance.  
  - Compare raw vs. augmented images.  

- **Model Development**  
  - Baseline: **ResNet50** pretrained on ImageNet.  
  - Fine-tuning with custom dense layers.  
  - Evaluate with accuracy, loss, and confusion matrix.
    
- **Deployment**  
  - Wrapped into a **Flask web app**.  
  - Users can upload dental X-ray or image scans.  
  - Model performs inference and returns the **predicted disease category** in real time.      
---

## 🛠️ Technology Stack  

- **Language:** Python 3.x  
- **Frameworks:** TensorFlow, Keras  
- **ML Libraries:** Scikit-learn, OpenCV  
- **Visualization:** Matplotlib, Seaborn  
- **Environment:** Kaggle / Google Colab (GPU-enabled)  

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white"/>
  <img src="https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white"/>
  <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white"/>
  <img src="https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white"/>
  <img src="https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge&logo=plotly&logoColor=white"/>
</p>  

---
## 👨‍💻 Author  

✨ **𝑬𝒏𝒈. 𝒫𝒶𝓊𝓁𝒶 𝐻𝒶𝓃𝓃𝒶 𝒩𝒶𝑔𝓊𝒾𝒷** ✨  

📌 *“𝒦𝓃𝓸𝓌𝓁𝑒𝒹𝑔𝑒 𝒾𝓈 𝓅𝑜𝓌𝑒𝓇. 𝒜𝓅𝓅𝓁𝓎𝒾𝓃𝑔 𝒜𝐼 𝓉𝑜 𝒽𝑒𝒶𝓁𝓉𝒽𝒸𝒶𝓇𝑒 𝓉𝓇𝒶𝓃𝓈𝒻𝑜𝓇𝓂𝓈 𝒾𝓃𝒻𝑜𝓇𝓂𝒶𝓉𝒾𝑜𝓃 𝒾𝓃𝓉𝑜 𝓁𝒾𝒻𝑒-𝒸𝒽𝒶𝓃𝑔𝒾𝓃𝑔 𝒾𝓃𝓈𝒾𝑔𝒽𝓉𝓈.”*  

