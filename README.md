# Motor Imagery Classification for Brain-Computer Interfaces

![Project Banner](bci.jpg)

## Overview
This project, **Motor Imagery Classification for Brain-Computer Interfaces Using EEGNetv4**, focuses on decoding electroencephalogram (EEG) signals to predict imagined hand movements (left vs. right). By leveraging the **EEGNetv4** model, a compact convolutional neural network (CNN), the project aims to advance Brain-Computer Interface (BCI) systems for applications in assistive technology, neurorehabilitation, and human-computer interaction.

The project uses the **BCI Competition IV Dataset 1**, which contains EEG recordings from subjects performing motor imagery tasks. The model is trained to classify left-hand vs. right-hand movements, handling challenges like noisy EEG signals and class imbalance using class weights. Performance is evaluated through accuracy, confusion matrices, and visualizations of predicted labels and EEG signals.

## Features
- **EEGNetv4 Model**: A lightweight CNN designed for EEG signal classification, capturing spatial and temporal features.
- **Dataset**: BCI Competition IV Dataset 1 with EEG data sampled at 1000 Hz.
- **Preprocessing**: EEG signal filtering, segmentation, and normalization for robust feature extraction.
- **Evaluation**: Metrics include accuracy, confusion matrices, and visualizations (scatter plots, histograms, and EEG signal plots).
- **Applications**: Potential use in voice-based authentication, customer service automation, speech assessment, and healthcare monitoring (adapted from voice classification insights).

## Dataset
The **BCI Competition IV Dataset 1** includes:
- EEG recordings from multiple subjects performing left-hand and right-hand motor imagery tasks.
- Calibration (training) and evaluation (testing) data.
- 1000 Hz sampling frequency with multiple channels, focusing on motor cortex-related channels (e.g., C3, Cz, C4).

## Installation
To run this project locally, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/motor-imagery-bci.git
   cd motor-imagery-bci
