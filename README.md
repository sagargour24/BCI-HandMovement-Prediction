# EEG-Based Motor Imagery Classification

This project involves using deep learning techniques to classify motor imagery EEG signals (left vs. right hand movement imagery) using a convolutional neural network (CNN). The model predicts motor intent from EEG data and is evaluated on a test dataset.

---

## 🧠 Project Overview

Electroencephalography (EEG) signals are used to interpret motor intentions in brain-computer interface (BCI) applications. This project aims to:

- Preprocess EEG data  
- Train a deep CNN model  
- Classify motor imagery (left vs. right)  
- Visualize model predictions and performance  

---

## 🗃️ Dataset

- Input shape: `(n_channels, n_times)` per trial  
- Channels used: `ch3`, `ch4`, `ch5`  
- Labels:  
  - `0` = Left imagery  
  - `1` = Right imagery  
- Data is structured into trials with temporal sequences  

---

## 🧠 Model Architecture

The deep learning architecture consists of temporal and spatial convolutional layers followed by pooling, dropout, and a dense classification layer.

<p align="center">
  <img src="images/model_architecture.jpg" alt="Model Architecture" width="250">
</p>

---

## 📊 Results & Visualizations

### Label Distribution

Distribution of predicted labels on the evaluation dataset:

<p align="center">
  <img src="images/label_distribution.jpg" alt="Label Distribution" width="400">
</p>

---

### Predicted Labels Across All Trials

Visualizing all predicted labels against trial numbers:

<p align="center">
  <img src="images/predicted_labels_all_trials.jpg" alt="All Predicted Labels" width="600">
</p>

---

### Sample Trial Predictions (Correct)

EEG waveforms for a few trials where predictions match the true labels:

<p align="center">
  <img src="images/sample_correct_predictions.jpg" alt="Correct Predictions" width="700">
</p>

---

### Sample Trial Predictions (Incorrect)

EEG waveforms for a few trials where predictions are incorrect:

<p align="center">
  <img src="images/sample_incorrect_predictions.jpg" alt="Incorrect Predictions" width="900">
</p>

---

## 📂 Files

- `EEG.ipynb`: Jupyter notebook with data processing, model training, evaluation, and visualization  
- `images/`: Contains all the result and architecture images

---

## 🚀 How to Run

1. Clone this repository  
2. Open `EEG.ipynb` in Jupyter Notebook or Google Colab  
3. Run all cells to:
   - Preprocess EEG data  
   - Train the CNN  
   - Evaluate predictions  

---

## 🧪 Future Work

- Add more EEG channels or frequency-domain features  
- Explore transformer or attention-based models  
- Integrate for real-time BCI feedback  

---

## 📬 Contact

For feedback or questions, please open an issue on this repository.

---

### ✅ Image File Mapping (Rename Your Files to These)

Place these renamed files in an `images/` folder:

| Current Filename                          | Rename to                          |
|-------------------------------------------|------------------------------------|
| `IMG-20250522-WA0001.jpg`                 | `predicted_labels_all_trials.jpg`  |
| `IMG-20250522-WA0002.jpg`                 | `sample_correct_predictions.jpg`   |
| `IMG-20250522-WA0003.jpg`                 | `sample_incorrect_predictions.jpg` |
| `IMG-20250522-WA0004.jpg`                 | `model_architecture.jpg`           |
| `IMG-20250522-WA0006.jpg`                 | `label_distribution.jpg`           |
