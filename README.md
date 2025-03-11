# Siamese Neural Network - Face Similarity Detection

<img src="siamese_visual.webp" alt="Siamese Network Visualization" width="60%"/>

## Overview
This project implements a Siamese Neural Network to detect face similarity by comparing pairs of grayscale images. The network learns to determine whether two images belong to the same person, using deep learning techniques and performance-boosting enhancements.

## Key Features
- **Siamese Architecture** based on convolutional layers and dense embeddings.
- **Multiple Model Variants**: Base model + improved versions with batch normalization, dropout, L2 regularization, and early stopping.
- **Data Augmentation**: Rotation, flipping, brightness and contrast variations.
- **Hyperparameter Tuning**: Grid search on learning rate, batch size, epochs, and early stopping.
- **Evaluation Metrics**: Accuracy, loss, and generalization performance on unseen test data.

## Technologies Used
- Python, PyTorch, NumPy

## Project Structure
- `ass2_notebook.ipynb` – Main implementation and training notebook
- `ass2 - report.pdf` – Full written report with results, analysis, and design rationale

## Experiments Summary
| Experiment | Accuracy | Loss | Key Additions                            |
|-----------|----------|------|-----------------------------------------|
| Base      | 66.00%   | 0.715 | Reference paper architecture             |
| Model 1   | 75.00%   | 0.550 | BatchNorm, Data Augmentation             |
| Model 2   | 52.90%   | 0.659 | Dropout, L2 Regularization, LR Scheduler |
| Model 3   | 72.60%   | 0.545 | Early Stopping, MSELoss                 |

## Setup Instructions
1. Clone the repository:
```bash
git clone https://github.com/your-username/siamese-network-face-similarity.git
cd siamese-network-face-similarity
```
2. Install dependencies:
```bash
pip install -r requirements.txt
```
3. Run the notebook in your preferred environment (Jupyter/Colab).

## Final Notes
The project demonstrates iterative model improvements through empirical experimentation, showcasing the importance of architecture tuning and training strategies in deep learning tasks.

