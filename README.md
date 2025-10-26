
# Waste detection and classification deep learning

## Overview
This project focuses on developing and evaluating deep learning models for the **detection and classification of waste materials** from images.  
It aims to support the automation of waste sorting and recycling processes by identifying different types of trash, such as **plastic, paper, metal, glass, and organic waste**, through computer vision techniques.

The work is carried out as part of the *Machine and Deep Learning* module in the **VIBOT MSc – Computer Vision and Robotics** program at the **Université de Bourgogne**.

---

## Objective
To build a robust image-based classification model capable of distinguishing waste categories using both **custom CNN architectures** and **transfer learning models**.  
Performance will be compared across different architectures to analyze trade-offs between accuracy, inference time, and generalization.

---

## Methodology

### 1. Dataset
- **Dataset:** [TrashNet](https://github.com/garythung/trashnet)  
- **Classes:** Paper, Cardboard, Plastic, Metal, Glass, and Trash  
- **Preprocessing:**
  - Image resizing and normalization  
  - Data augmentation (rotation, flips, brightness adjustments)  
  - Train-validation-test split for evaluation consistency

### 2. Model Development
- **Baseline:** Transfer learning using pretrained CNN backbones (e.g., ResNet, EfficientNet)  
- **Custom Head:** Designed a lightweight classifier with dropout and batch normalization layers for improved regularization  
- **Loss Function:** CrossEntropyLoss  
- **Optimizer:** Adam / SGD with dynamic learning rate scheduling  
- **Evaluation Metrics:** Accuracy, Precision, Recall, F1-Score  

### 3. Experimentation
- Conducted experiments to compare:
  - Custom model vs. pretrained models  
  - Impact of data augmentation on accuracy  
  - Training time vs. performance trade-offs  
- Visualized training curves and confusion matrices for interpretability.

---

## Tools and Frameworks
- **Language:** Python  
- **Framework:** PyTorch  
- **Libraries:** NumPy, OpenCV, Matplotlib, Scikit-learn  
- **Environment:** Jupyter Notebook / Google Colab  

---

## Current Progress
The dataset pipeline and baseline models have been set up successfully.  
The custom classifier head is under development, and experiments comparing transfer learning models are ongoing.  
Model checkpoints and evaluation plots will be added as training progresses.

---

## Future Work
- Hyperparameter optimization and fine-tuning  
- Integration of object detection (e.g., YOLOv8) for real-time classification  
- Deployment-ready lightweight model export (ONNX / TorchScript)  
- Extension toward robotic waste sorting applications  

---

## Repository Structure
```
waste-classification/
│
├── data/                # Dataset and splits
├── notebooks/           # Jupyter notebooks for experiments
├── src/                 # Model architecture and training scripts
├── outputs/             # Model checkpoints and logs
├── results/             # Evaluation metrics and visualizations
└── README.md
```

---

## Authors
**Muhammad Usama Javaid**  
MSc – Computer Vision & Robotics (VIBOT)  
Université de Bourgogne  
[LinkedIn](https://www.linkedin.com/in/imusama/) | [GitHub](https://github.com/imusama1)


**Team Members:**

  * [Ahmed Khalil](https://github.com/ahmad-laradev)


---

## License
This repository is created for academic and research purposes under the VIBOT MSc program.  
Use or reference is permitted with proper credit.
```


