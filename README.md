# Emotion-detection-using-EEG-Brainwave-dataset
**Description:**

This project investigates the efficacy of a hybrid deep learning model for classifying emotional states using Electroencephalogram (EEG) brainwave data. The dataset, sourced from Kaggle's "EEG brainwave dataset: mental state," contains EEG recordings from four participants (two male, two female) in three emotional states: relaxed, concentrating, and neutral. Each recording spans 60 seconds.

**Data Preprocessing:**

* Feature Scaling: The data undergoes standardization using a StandardScaler to ensure features have a mean of 0 and a standard deviation of 1. This facilitates training by mitigating the impact of features with vastly different scales.
* Dimensionality Reduction: Principal Component Analysis (PCA) is employed to reduce the data's dimensionality while retaining the most relevant information. This step enhances computational efficiency and potentially helps prevent overfitting by reducing the number of features the model needs to learn.

**Model Architecture:**

* Hybrid Deep Learning: The model combines two powerful deep learning techniques:
* Convolutional Neural Network (CNN): This component effectively captures spatial relationships and feature patterns within EEG signals.
* Bidirectional Long Short-Term Memory (BiLSTM): This component excels at learning temporal dependencies and sequential information in the dynamic EEG data, particularly crucial for emotion classification.

**Training and Evaluation:**

* The model is trained on the preprocessed EEG data.
* Performance is evaluated using a standard metric such as training, testing, validation accuracy. The reported testing accuracy of 94.86% indicates a highly promising capability to distinguish among the three emotional states.
* Other performance metrics such as classification report, confusion matrix, ROC - AUC Curves, Model accuracy, loss and AUC graphs are also considered.

**Dataset source:**
https://www.kaggle.com/datasets/birdy654/eeg-brainwave-dataset-mental-state/data
