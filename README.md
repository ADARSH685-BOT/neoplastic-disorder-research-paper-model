# 🧠 Neoplastic Disorder ML Model
## Brain Tumor Classification using Deep Learning

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange.svg)](https://www.tensorflow.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-green.svg)](https://jupyter.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Stars](https://img.shields.io/github/stars/owner/repo?style=social)](https://github.com/owner/repo)

This project implements a **Convolutional Neural Network (CNN)** for classifying brain tumors from MRI images, focusing on neoplastic disorders. Built as a research paper prototype using synthetic data for demonstration.

## ✨ Features
- **4-Class Classification**: Glioma, Meningioma, No Tumor, Pituitary
- **Synthetic Dataset**: 200 images (50 per class, train/test split)
- **End-to-End Pipeline**: Data prep, training, evaluation, visualizations
- **Performance**: ~87% accuracy on validation set

## 📊 Dataset Overview
| Class       | Train Images | Test Images |
|-------------|--------------|-------------|
| Glioma      | 50           | 50          |
| Meningioma  | 50           | 50          |
| No Tumor    | 50           | 50          |
| Pituitary   | 50           | 50          |

![Class Distribution](./Figure2_ClassDistribution.png)

## 🏗️ Model & Training
- **Framework**: TensorFlow/Keras
- **Epochs**: 15
- **Results**:

![Accuracy & Loss](./Figure3_Accuracy.png)
![Loss Curves](./Figure4_Loss.png)

## 📈 Evaluation Metrics
![Confusion Matrix](./Figure5_ConfusionMatrix.png)

![ROC Curves](./Figure_ROC.png)

**Confusion Matrix**:
```
Actual \ Pred | Glioma | Meningioma | No Tumor | Pituitary
--------------|--------|------------|----------|----------
Glioma        | 18     | 1          | 0        | 1
Meningioma    | 2      | 16         | 1        | 1
No Tumor      | 1      | 2          | 15       | 2
Pituitary     | 0      | 1          | 2       | 17
```

## 🚀 Quick Start
1. Install dependencies:
   ```
   pip install tensorflow matplotlib scikit-learn pillow seaborn numpy
   ```
2. Run the notebook:
   ```
   jupyter notebook neoplastic_disorder_model.ipynb
   ```
3. Execute all cells to generate data, train, and visualize.

**Note**: Uses synthetic data. Replace with real MRI dataset (e.g., Brain Tumor Dataset on Kaggle) for production.

## 📁 Project Structure
```
.
├── neoplastic_disorder_model.ipynb  # Main notebook
├── Figure1_SampleImages.png         # Generated figures
├── README.md                        # This file
└── TODO.md                          # Progress tracking
```

## 🔮 Future Work
- Integrate real MRI dataset
- Advanced CNN (ResNet, EfficientNet)
- Deployment (TensorFlow Lite/Streamlit)
- Cross-validation & Hyperparameter tuning

## 🤝 Contributing
Contributions welcome! Fork, PR, or open issues.

## 📄 License
MIT License - see [LICENSE](LICENSE) for details.

---

**Built with ❤️ for Neoplastic Disorder Research**  
*Adarsh Kumar | 2024*

