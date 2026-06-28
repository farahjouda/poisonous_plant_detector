#  Poisonous Plant Detection using Deep Learning

## Project Overview

This project presents a deep learning-based image classification system for detecting whether a plant is **Poisonous** or **Non-Poisonous** from leaf images. The model is built using **PyTorch** and leverages **Transfer Learning** with EfficientNet-B2 to improve classification performance while reducing training time. The project includes data preprocessing, model training, fine-tuning, evaluation, and prediction visualization.

---

## Objectives

- Build a deep learning model for poisonous plant detection.
- Apply transfer learning using a pretrained EfficientNet-B2 model.
- Fine-tune the model to improve classification performance.
- Evaluate the model using multiple performance metrics.
- Save the trained model for future inference and deployment.

---

## Features

- Binary image classification (Poisonous / Non-Poisonous)
- Transfer Learning using EfficientNet-B2
- Two-stage training and fine-tuning
- Image preprocessing and normalization
- Custom PyTorch Dataset and DataLoader
- AdamW optimizer
- Learning rate scheduling
- Early stopping
- Model checkpoint saving
- Accuracy and loss visualization
- Confusion Matrix
- Classification Report
- Prediction visualization on test images

---

## Dataset

The dataset contains labeled images of poisonous and non-poisonous plants.

Dataset splits include:

- Training Set
- Validation Set
- Test Set

The project also visualizes the distribution of classes before training.

---

## Data Preprocessing

The preprocessing pipeline includes:

- Image resizing
- Image normalization
- Tensor conversion
- Dataset splitting
- Custom Dataset implementation
- DataLoader optimization

---

## Model Architecture

The project uses **EfficientNet-B2** pretrained on ImageNet as the backbone model.

The classifier was customized by adding:

- Dropout Layer
- Fully Connected Layer
- SiLU Activation
- Batch Normalization
- Output Layer for binary classification

---

## Training Strategy

The model was trained in two stages:

### Stage 1

- Freeze pretrained backbone layers.
- Train only the custom classifier.

### Stage 2

- Unfreeze selected EfficientNet layers.
- Fine-tune the network using a lower learning rate.

Training techniques include:

- AdamW Optimizer
- CrossEntropy Loss
- ReduceLROnPlateau Scheduler
- Early Stopping
- Best Model Checkpoint

---

## Evaluation

The trained model is evaluated using:

- Classification Accuracy
- Confusion Matrix
- Classification Report
- Training Accuracy Curve
- Validation Accuracy Curve
- Training Loss Curve
- Validation Loss Curve

The project also demonstrates predictions on unseen plant images.

---

## Technologies Used

- Python
- PyTorch
- TorchVision
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Pillow
- Google Colab

---

## Project Structure

```text
PoisonousPlantDetector/
│
├── poisonous_plant_detector.ipynb
├── README.md
```

---

## How to Run

Install the required libraries:

```bash
pip install torch torchvision pandas numpy matplotlib seaborn scikit-learn pillow
```

Run the notebook:

```bash
jupyter notebook poisonous_plant_detector.ipynb
```

or open it directly in Google Colab.

---

## Learning Outcomes

This project demonstrates practical experience with:

- Deep Learning
- Image Classification
- Transfer Learning
- EfficientNet
- Fine-Tuning
- PyTorch
- Data Preprocessing
- Model Evaluation
- Computer Vision

---

## Future Improvements

- Increase dataset size.
- Support additional plant species.
- Deploy the model as a web application.
- Develop a mobile application for real-time plant identification.
- Integrate explainable AI techniques such as Grad-CAM.

---

## Author

**Farah Jouda**

Bachelor of Computer Science and Information Systems

Major: Artificial Intelligence

---


