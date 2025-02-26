# gait_classification
# Gait Classification using Deep Learning

## Overview
This project explores deep learning methods for pathological gait classification using 3D skeleton and foot pressure data. The study investigates various architectures, including GRU-based and CNN-based models, and evaluates computational efficiency and classification performance.

## Project Files
- `gait_classification.ipynb` - Main Jupyter Notebook containing data preprocessing, model training, evaluation, and results analysis.
- `requirements.txt` - List of dependencies needed to run the notebook.

## Datasets
This study utilizes two complementary datasets:

1. **3D Skeleton Dataset** (captured using Azure Kinect)  
   - Tracks 32 joint coordinates over time.
   - 6 gait patterns (1 normal + 5 pathological).

2. **Foot Pressure Dataset** (collected with GW1100 pressure plate)  
   - Captures average foot pressure per step.

## Deep Learning Models
The notebook explores multiple architectures for gait classification:
- **1D Convolutional Autoencoder (1D CAE)** - Feature extraction from gait sequences.
- **GRU Model** - Sequential model capturing temporal dependencies.
- **GRU-CNN Hybrid Model** - Incorporates both skeleton and foot pressure data.
- **CNN Models** - Capture spatial dependencies in gait patterns.

### Key Findings
- CNN models trained faster but consumed more memory and CPU power.
- GRU-based models took longer to train but had lower computational load.
- CNN2 achieved the best classification performance.

## Installation and Setup

### Clone the repository
```bash
git clone https://github.com/alisasnezskaia/gait_classification.git
cd gait_classification
