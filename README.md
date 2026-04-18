# Garbage Classification & Bin Navigator

A deep learning project that classifies waste images into 6 categories
and recommends the correct disposal bin using CNN and ResNet18 transfer
learning. Built with PyTorch for ADSC 4720 - Data Mining in Applied
Data Science.

## Project Overview

Improper waste disposal is a growing environmental problem. This project
builds a deep learning pipeline that:
1. Classifies a garbage image into one of 6 categories
2. Recommends the correct disposal bin based on Metro Vancouver guidelines
3. Demonstrates potential for robotic waste sorting systems

## Dataset

- **Source:** [Kaggle Garbage Classification](https://www.kaggle.com/datasets/asdasdasasdas/garbage-classification)
- **Size:** 2,527 images across 6 classes
- **Classes:** Cardboard, Glass, Metal, Paper, Plastic, Trash

## Results

| Model | Val Accuracy | Test Accuracy |
|---|---|---|
| Baseline CNN (scratch) | 61.5% | — |
| ResNet18 (transfer learning) | 90.2% | 90.5% |

## Project Structure

garbage-classifier/
│
├── data/                        ← dataset (not tracked by git)
├── notebooks/
│   └── garbage_classifier.ipynb ← main notebook
├── outputs/
│   ├── models/                  ← saved model weights
│   └── plots/                   ← saved figures
├── requirements.txt
├── .gitignore
└── README.md

## Notebook Structure

1. Problem Definition & Goals
2. Exploratory Data Analysis
3. Preprocessing & Data Augmentation
4. Baseline CNN Model
5. ResNet18 Transfer Learning
6. Evaluation & Results
7. Bin Navigator
8. Conclusion

## How to Run

### Option 1 — Google Colab (recommended)
1. Open `notebooks/garbage_classifier.ipynb` in Google Colab
2. Enable GPU: Runtime → Change runtime type → T4 GPU
3. Mount Google Drive and set dataset path
4. Run all cells in order

### Option 2 — Local (VS Code)
1. Clone the repository:
git clone https://github.com/BVishwa12/garbage-classifier.git

2. Install dependencies:

pip install -r requirements.txt

3. Download dataset from Kaggle and place in `data/garbage_classification/`
4. Open `notebooks/garbage_classifier.ipynb` in VS Code
5. Run all cells in order

## Requirements

See `requirements.txt` for full list. Key dependencies:
- torch
- torchvision
- matplotlib
- seaborn
- scikit-learn
- pillow
- numpy

## Real World Applications

- Mobile app for instant waste disposal guidance
- Robotic sorting systems in recycling facilities
- Smart city waste management analytics

## Course

ADSC 4720 - Data Mining in Applied Data Science
Thompson Rivers University — Winter 2026
