🦷 Teeth Classification & Disease Detection
📌 Project Overview

This project focuses on developing a deep learning-based solution for teeth classification and disease detection.
The pipeline includes preprocessing, visualization, model training, and evaluation to classify dental images into 7 categories:

CaS – Cavity Stage

CoS – Composite Stage

Gum – Gum Issues

MC – Missing Crown

OC – Oral Cavity

OLP – Oral Lichen Planus

OT – Other Teeth issues

This solution supports AI-driven healthcare applications, enhancing diagnostic accuracy and improving patient treatment planning.

🎯 Objectives

Preprocessing

Normalize and resize images to 256x256.

Apply augmentation (flips, brightness, contrast, saturation) for dataset diversity.

Visualization

Display random samples per category.

Visualize class distribution (bar chart).

Compare images before vs after augmentation.

Model Development

Train a baseline CNN using ResNet50 (transfer learning).

Establish a performance baseline with metrics (accuracy, loss, confusion matrix).

Fine-tune for improved results.

🛠️ Tech Stack

Language: Python 3

Frameworks: TensorFlow, Keras

ML/DL Libraries: scikit-learn, OpenCV, Albumentations

Visualization: Matplotlib, Seaborn

Hardware: GPU/TPU (Kaggle/Colab)
