# 🌱 Plant Disease Detection using Deep Learning

## 📌 Overview
This project focuses on building a **deep learning-based plant disease detection system** using **Convolutional Neural Networks (CNNs)**. The goal is to classify plant leaf images into healthy or diseased categories, providing farmers and researchers with an efficient tool for early detection and prevention.  

The project emphasizes:
- **Reproducibility**: Clear structure and documentation for academic submission.  
- **Explainability**: Using **Grad-CAM** to visualize model decisions.  
- **Practicality**: A simple demo interface to showcase real-world usability.  

---

## 📂 Project Structure
```
├── data/                # Raw dataset (leaf images)
├── split_data/           # Train/test splits
├── notebooks/            # Step-by-step workflow
│   ├── 01_dataset_preprocessing.ipynb
│   ├── 02_model_training.ipynb
│   ├── 03_gradcam_explainability.ipynb
│   └── 04_interface_demo.ipynb
├── models/              # Trained weights (saved models)
├── results/             # Accuracy/loss plots & Grad-CAM outputs
├── README.md            # Project documentation
└── LICENSE              # MIT License
```

---

## ⚙️ Workflow
1. **Dataset Preprocessing**  
   - Image resizing, normalization, and augmentation.  
   - Train/test split stored in `split_data/`.  

2. **Model Training**  
   - CNN/Transfer Learning (e.g., ResNet, EfficientNet).  
   - Training logs, accuracy, and loss curves saved in `results/`.  

3. **Explainability with Grad-CAM**  
   - Visualizing which regions of the leaf influenced predictions.  
   - Outputs stored in `results/gradcam/`.  

4. **Interface Demo**  
   - Simple notebook-based interface for testing new leaf images.  
   - Upload an image → get prediction + Grad-CAM visualization.  

---

## 📊 Results
- Achieved **high accuracy** on test data.  
- Grad-CAM overlays show that the model focuses on diseased regions of leaves.  
- Accuracy/Loss plots demonstrate stable training with minimal overfitting.  

---

## 🚀 Getting Started
### Prerequisites
- Python 3.8+  
- Jupyter Notebook  
- Libraries: `tensorflow`, `keras`, `numpy`, `matplotlib`, `opencv-python`, `scikit-learn`

### Installation
```bash
git clone https://github.com/yourusername/plant-disease-detection.git
cd plant-disease-detection
pip install -r requirements.txt
```

### Running the Workflow
1. Open `notebooks/01_dataset_preprocessing.ipynb` → preprocess dataset.  
2. Run `notebooks/02_model_training.ipynb` → train CNN model.  
3. Use `notebooks/03_gradcam_explainability.ipynb` → generate Grad-CAM visualizations.  
4. Try `notebooks/04_interface_demo.ipynb` → test with custom images.  

---

## 📜 License
This project is licensed under the **MIT License** – free to use, modify, and distribute with attribution.  

---

## 🎯 Future Work
- Collect a larger dataset with more plant species.
- Experiment with advanced architectures (EfficientNet, Vision Transformers).
- Deploy as a web/mobile app for farmers.
- Integrate with IoT sensors for real-time monitoring.
- Explore other explainability methods beyond Grad-CAM.
