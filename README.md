# Ocular Disease Detection using Deep Learning

This project implements a deep learning-based framework for the classification of ocular diseases from retinal fundus images. The current implementation focuses on binary classification of cataract vs. normal cases, but the architecture is designed to scale for multi-class detection of other ocular conditions such as glaucoma, diabetic retinopathy, and age-related macular degeneration.

## Overview

Developed as part of an independent research initiative at Netaji Subhas University of Technology, this project evaluates the performance of multiple deep learning models—both with and without classical image preprocessing techniques.

### Key Features:
- Dataset: ODIR (Ocular Disease Intelligent Recognition)
- Focus: Binary classification (Cataract vs. Normal)
- Models: VGG-19, ResNet50, Vision Transformer (ViT)
- Preprocessing: Local Binary Pattern (LBP) for texture enhancement
- Output: Model performance metrics and a research paper based on the experiments

## Methodology

- Reformulated the original multi-class problem into a binary task
- Applied LBP preprocessing to improve texture-level features
- Trained and validated deep models on both raw and LBP-enhanced images
- Evaluated performance based on validation accuracy and confusion matrices

## Results

| Model              | Accuracy (Raw Images) | Accuracy (With LBP) |
|--------------------|-----------------------|----------------------|
| VGG-19             | 83.33%                | 94.44%               |
| ResNet50           | 87.50%                | 100%                 |
| Vision Transformer | 71.43%                | 85.71%               |

ResNet50 with LBP preprocessing achieved the highest validation accuracy of **100%**.

## Tech Stack

- Python
- PyTorch
- OpenCV
- Matplotlib
- Jupyter Notebooks

## Project Structure

- `/notebooks/` – Training, evaluation, and analysis notebooks
- `/paper/` – Research paper detailing the methodology and results
- `/plots/` – Visualizations and confusion matrices (optional)

## Research Paper

A formal research paper based on this project is included in the `/research` directory:


## License

This project is provided for academic and educational use only.
