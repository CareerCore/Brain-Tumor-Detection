# 🧠 Brain Tumor MRI Classification using EfficientNet-B2 (PyTorch)

A deep learning project for **binary brain tumor classification** from MRI images using **EfficientNet-B2** and **PyTorch**. This project classifies MRI scans into:

- 🟢 Healthy
- 🔴 Tumor

The model uses **transfer learning**, **early stopping**, and **learning rate scheduling** to achieve high classification performance.

---

# 📌 Features

- Binary Classification (Healthy vs Tumor)
- EfficientNet-B2 Transfer Learning
- PyTorch Implementation
- Data Augmentation
- Early Stopping
- Learning Rate Scheduler
- Best Model Checkpoint Saving
- Training & Validation Accuracy Graph
- Training & Validation Loss Graph
- Confusion Matrix
- Classification Report
- ROC Curve & AUC Score
- Single Image Prediction
- Google Colab Compatible

---

# 📂 Dataset Structure

```
Brain Tumor MRI Images/
│
├── Healthy/
│   ├── image1.jpg
│   ├── image2.jpg
│   └── ...
│
└── Tumor/
    ├── image1.jpg
    ├── image2.jpg
    └── ...
```

---

# 📊 Dataset Information

- Classes: 2
- Healthy
- Tumor

The dataset is automatically divided into:

- 70% Training
- 15% Validation
- 15% Testing

---

# 🏗️ Model Architecture

- EfficientNet-B2 (Pretrained on ImageNet)
- Transfer Learning
- Custom Classification Head

```
EfficientNet-B2
        │
Global Feature Extractor
        │
Fully Connected Layer
        │
2 Output Classes
```

---

# ⚙️ Training Configuration

| Parameter | Value |
|-----------|---------|
| Framework | PyTorch |
| Model | EfficientNet-B2 |
| Epochs | 30 |
| Batch Size | 16 |
| Optimizer | Adam |
| Learning Rate | 1e-4 |
| Loss Function | CrossEntropyLoss |
| Scheduler | ReduceLROnPlateau |
| Early Stopping | Yes |

---

# 📈 Evaluation Metrics

The project evaluates the model using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- ROC Curve
- AUC Score
- Classification Report

---

# 📉 Training Graphs

The notebook generates:

- Training Loss
- Validation Loss
- Training Accuracy
- Validation Accuracy

These graphs help visualize the learning progress of the model.

---

# 💾 Saved Model

The best model is automatically saved during training.

```
best_model.pth
```

or

```
Models/
    best_model.pth
```

---

# 🔍 Testing

The notebook includes a prediction script that allows the user to:

- Upload an MRI image
- Predict Healthy or Tumor
- Display prediction confidence
- Display uploaded image

Example Output:

```
Prediction : Tumor

Confidence : 99.84%
```

---

# 📁 Project Structure

```
Brain-Tumor-MRI-Classification/

│
├── MRI_Brain_Tumor_Detection_B2.ipynb
├── README.md
├── best_model.pth
├── requirements.txt
├── Dataset/
│
├── Models/
│   └── best_model.pth
│
├── Results/
│   ├── accuracy.png
│   ├── loss.png
│   ├── confusion_matrix.png
│   └── roc_curve.png
│
└── Sample Images/
```

---

# 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/Brain-Tumor-MRI-Classification.git
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

# ▶️ Run

Open the notebook:

```
MRI_Brain_Tumor_Detection_B2.ipynb
```

Run all cells sequentially.

---

# 📦 Required Libraries

```
torch
torchvision
numpy
matplotlib
scikit-learn
Pillow
tqdm
```

Install manually:

```bash
pip install torch torchvision numpy matplotlib scikit-learn pillow tqdm
```

---

# 🎯 Results

The model achieved:

- High Training Accuracy
- High Validation Accuracy
- Efficient Binary Classification
- Lightweight and Fast Inference

---

# 📚 Technologies Used

- Python
- PyTorch
- TorchVision
- Google Colab
- NumPy
- Matplotlib
- Scikit-learn
- PIL

---

# 📜 License

This project is developed for educational and research purposes.

---

# 👨‍💻 Author

**Muhammad Arslan**

Computer Science Student

Deep Learning | Computer Vision | Artificial Intelligence

---

⭐ If you found this project useful, consider giving it a star on GitHub!
