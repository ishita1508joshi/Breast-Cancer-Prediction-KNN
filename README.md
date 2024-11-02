# Breast Cancer Prediction using K-Nearest Neighbors (KNN)
This project applies the K-Nearest Neighbors (KNN) algorithm to classify tumors as malignant or benign based on the Breast Cancer Wisconsin dataset. By training and testing the model, this project aims to achieve high accuracy in distinguishing between the two classes, using patient features such as radius, texture, perimeter, and area of cell nuclei.
### Project Files
- Breast Cancer Prediction using KNN.ipynb: Jupyter Notebook with the full code for loading the data, preprocessing, training the KNN model, and evaluating its performance.
- BreastCancerWisconsinDataset.csv: Dataset containing features of cell nuclei, each labeled as malignant (M) or benign (B).
### Dataset
The Breast Cancer Wisconsin dataset includes 30 features representing characteristics of cell nuclei from digitized images. Each instance is labeled as malignant or benign.
- Target Variable:
    - diagnosis: 1 for Malignant, 0 for Benign.
### Features and Methodology
1. Data Preprocessing:
- Dropped unnecessary columns (id, Unnamed: 32).
- Converted diagnosis labels to numerical values: Malignant (M) as 1 and Benign (B) as 0.
- Scaled features to ensure fair contribution to distance calculations in the KNN model.
2. Model Training:
- Implemented a KNN model with 5 neighbors, using Minkowski distance with p=2 (equivalent to Euclidean distance).
- Split the dataset into training (70%) and testing (30%) sets.
3. Performance Evaluation:
- Evaluated accuracy, precision, recall, and F1-score.
- Achieved an accuracy of 95.9% on the test set.
4. Visualization:
- Visualized decision boundaries on both training and test sets using only two features (radius_mean and texture_mean) for clarity.
### Results
- The model achieved 95.9% accuracy on the test set.
- Confusion matrix and classification report show strong performance in classifying both malignant and benign cases.
