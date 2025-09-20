🦷 Teeth Classification & Disease Detection
📖 Overview

This project develops a computer vision pipeline for automatic teeth classification and disease detection using deep learning. The system integrates data preprocessing, visualization, model training, and evaluation, enabling the classification of dental images into seven categories:

CaS – Cavity Stage

CoS – Composite Stage

Gum – Gum Issues

MC – Missing Crown

OC – Oral Cavity

OLP – Oral Lichen Planus

OT – Other Teeth Conditions

This work contributes to the advancement of AI-driven dental solutions, enhancing diagnostic accuracy and supporting healthcare professionals in treatment planning.

🎯 Objectives

Preprocessing

Normalize and resize images to ensure consistency.

Apply data augmentation (flips, brightness, contrast, saturation) to improve model robustness.

Visualization

Display representative samples per class.

Analyze class distribution for dataset balance.

Compare raw vs augmented images to validate transformations.

Model Development

Implement a deep learning model tailored for dental image classification.

Train a baseline ResNet50 architecture and fine-tune for improved performance.

Evaluate using metrics such as accuracy, loss, and confusion matrix.

🛠️ Technology Stack

Language: Python 3.x

Frameworks: TensorFlow, Keras

Machine Learning Libraries: scikit-learn, OpenCV

Visualization Tools: Matplotlib, Seaborn

Compute Environment: Kaggle / Google Colab (GPU-enabled)

📂 Repository Structure
├── data/                        # Dataset (Training, Validation, Testing)
├── notebooks/                   # Jupyter/Colab notebooks
├── src/                         # Core source files
│   ├── preprocessing.py         # Data loading & preprocessing
│   ├── visualization.py         # Visualization utilities
│   ├── model.py                 # Model architecture definition
│   └── train.py                 # Training & evaluation pipeline
├── results/                     # Plots, confusion matrix, metrics
├── README.md                    # Project documentation
└── requirements.txt             # Dependencies

⚙️ Preprocessing Pipeline

Normalization: Pixel values scaled to [0,1].

Resizing: Images resized to 256x256.

Augmentation: Random flips, brightness/contrast/saturation adjustments.

def decode_img(path, label):
    img = tf.io.read_file(path)
    img = tf.image.decode_jpeg(img, channels=3)
    img = tf.image.resize(img, [256,256])
    img = tf.cast(img, tf.float32) / 255.0
    return img, label

📊 Data Visualization

Sample images per class (visual verification).

Class distribution chart (dataset balance).

Augmentation examples (before vs after).

🧠 Model Architecture

We utilized ResNet50 (pretrained on ImageNet) with fine-tuning:

base_model = ResNet50(
    input_shape=(256, 256, 3),
    weights='imagenet',
    include_top=False
)

model = models.Sequential([
    base_model,
    layers.GlobalAveragePooling2D(),
    layers.Dropout(0.3),
    layers.Dense(128, activation='relu'),
    layers.Dropout(0.3),
    layers.Dense(7, activation='softmax')
])


Optimizer: Adam

Loss Function: Sparse Categorical Crossentropy

Evaluation Metric: Accuracy

🚀 Training Strategy

Stage 1: Train classifier head with ResNet50 frozen.

Stage 2: Fine-tune entire network with a reduced learning rate (1e-5).

📌 Training enhancements:

Early stopping

Learning rate reduction on plateau

Model checkpointing

📈 Results
Training & Validation Performance

Plots illustrate accuracy and loss trends across epochs:

Final Test Evaluation

Test Accuracy: XX.XX%

Test Loss: X.XX

Confusion Matrix

🏥 Impact

This model:

Supports dentists with AI-assisted diagnosis.

Enhances treatment planning through precise disease identification.

Demonstrates the integration of AI in healthcare for improved outcomes.

🔮 Future Directions

Incorporate EfficientNet and Vision Transformers (ViT) for improved performance.

Apply hyperparameter optimization techniques.

Deploy as an interactive web or mobile application.

📜 License

This project is licensed under the MIT License. See the LICENSE
 file for details.

👨‍💻 Author

Your Name
NLP & Computer Vision Engineer

📌 “Knowledge is power. Applying AI to healthcare transforms information into life-changing insights.”
