# README: Cybersecurity Threat Classification Project

## Project Overview
This project implements a **Random Forest classifier** to detect cybersecurity threats using a network traffic dataset. The goal is to classify network intrusions and malicious activities accurately. The model is evaluated using **accuracy, precision, recall, and F1-score**, and visualizations such as confusion matrices and feature importance plots are provided.

## Prerequisites
Ensure you have the following dependencies installed:

- Python 3.x
- Jupyter Notebook
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Imbalanced-learn

You can install the required libraries using:
```sh
pip install pandas numpy scikit-learn imbalanced-learn
```
## Running the Code

- Step 1: Open the Jupyter Notebook
The code is provided in a Jupyter Notebook (Cybersecurity_Threat_Classification.ipynb). To open it, run the cells.

- Step 2: Load the Dataset
The dataset used UNSW-NB15 contains labeled network traffic data.
You can Download the dataset from [here](https://research.unsw.edu.au/projects/unsw-nb15-dataset)
Ensure the dataset file is available and update the file path in the notebook if necessary.

- Step 3: Preprocess the Data
Missing values are handled by imputation.
Numerical features are normalized using StandardScaler.
Irrelevant features (e.g., IP addresses) are removed.

- Step 4: Train the Model
The dataset is split into 80% training and 20% testing.
A Random Forest classifier is trained on the data.
Hyperparameters are optimized using Grid Search with 5-fold cross-validation.

- Step 5: Evaluate the Model
Metrics like accuracy, precision, recall, and F1-score are computed.
A confusion matrix and feature importance plot are generated.

- Step 6: Interpret Results
The model performs well on DoS attacks and port scans.
Performance on zero-day attacks is comparatively lower.
