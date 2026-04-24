# ML Brain Tumour Project

## 📋 Overview

This project implements deep learning models for **brain tumor detection, classification, and segmentation** using state-of-the-art computer vision techniques. We leverage CNN (Convolutional Neural Networks), YOLO (You Only Look Once), and Mask R-CNN to achieve high-accuracy tumor identification and boundary delineation.

### Project Goals
- 🎯 Detect and localize brain tumors in MRI images
- 📊 Classify tumor types with high accuracy
- 🔍 Segment tumor regions for precise boundary identification
- 📈 Provide interpretable results for medical professionals

---

## 🛠️ Technology Stack

| Technology | Purpose |
|-----------|---------|
| **CNN** | Feature extraction and classification |
| **YOLO** | Fast object detection and localization |
| **Mask R-CNN** | Instance segmentation and boundary detection |
| **Python** | Primary programming language |
| **TensorFlow/PyTorch** | Deep learning frameworks |
| **OpenCV** | Image processing |
| **Jupyter Notebook** | Interactive development and analysis |

---

## 📁 Project Structure

```
ML-Brain_tumour_project/
├── README.md                    # This file
├── notebooks/                   # Jupyter notebooks for analysis
│   ├── data_exploration.ipynb
│   ├── model_training.ipynb
│   └── inference_demo.ipynb
├── src/                         # Source code
│   ├── models/                  # Model implementations
│   ├── utils/                   # Utility functions
│   └── preprocessing/           # Data preprocessing scripts
├── data/                        # Dataset directory
│   ├── train/
│   ├── val/
│   └── test/
├── results/                     # Training results and visualizations
└── requirements.txt             # Python dependencies
```

---

## 🚀 Quick Start

### Prerequisites
- Python 3.8 or higher
- GPU support (CUDA) recommended for training
- pip or conda package manager

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/JtingF101/ML-Brain_tumour_project.git
cd ML-Brain_tumour_project
```

2. **Create a virtual environment**
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install dependencies**
```bash
pip install -r requirements.txt
```

### Data Preparation

1. Prepare your MRI image dataset
2. Organize images into `data/train`, `data/val`, and `data/test` directories
3. Ensure images are in standardized format (e.g., `.nii`, `.dcm`, `.jpg`)
4. Create corresponding annotation files if needed

### Training

```bash
# Run training notebook
jupyter notebook notebooks/model_training.ipynb

# Or run training script
python src/train.py --config config/model_config.yaml
```

### Inference

```bash
# Run inference on test images
python src/inference.py --input_path data/test/ --model_path models/best_model.pth
```

---

## 📚 Key Notebooks

- **`data_exploration.ipynb`** - Exploratory data analysis and visualization
- **`model_training.ipynb`** - Model training, validation, and hyperparameter tuning
- **`inference_demo.ipynb`** - Demonstration of inference on sample images

---

## 🔬 Methodology

### 1. Data Preprocessing
- Image normalization and standardization
- Augmentation techniques (rotation, flip, zoom)
- Train/validation/test split

### 2. Model Architecture
- **CNN**: Multi-layer convolutional network for feature extraction
- **YOLO**: Real-time detection with bounding box regression
- **Mask R-CNN**: Instance segmentation with pixel-level masks

### 3. Training Strategy
- Loss function optimization (Cross-entropy, Dice loss)
- Learning rate scheduling
- Early stopping to prevent overfitting
- Model ensemble for improved accuracy

### 4. Evaluation
- Confusion matrix analysis
- ROC-AUC curves
- Segmentation IoU (Intersection over Union)
- Clinical relevance assessment

---

## ⚠️ Important Disclaimer

**This project is for research and educational purposes only.** 

- Results should NOT be used for clinical diagnosis or treatment decisions
- Always consult qualified medical professionals for patient care
- This tool is meant to assist radiologists, not replace them
- Validation on diverse datasets is required before clinical deployment

---

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

This project is currently unlicensed. Please contact the author for licensing information.

---

## 📞 Contact & Support

- **Author**: [JtingF101](https://github.com/JtingF101)
- **Issues**: [GitHub Issues](https://github.com/JtingF101/ML-Brain_tumour_project/issues)
- **Discussions**: Feel free to open discussions for questions and ideas

---

## 🙏 Acknowledgments

- Dataset providers and medical collaborators
- Open-source communities (TensorFlow, PyTorch, OpenCV)
- Inspiration from state-of-the-art vision models

---

## 📖 References

- He, K., Gkioxari, G., Dollár, P., & Girshick, R. (2017). Mask R-CNN
- Redmon, J., & Farhadi, A. (2018). YOLOv3: An Incremental Improvement
- Krizhevsky, A., Sutskever, I., & Hinton, G. E. (2012). ImageNet Classification with Deep Convolutional Neural Networks

---
