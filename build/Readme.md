# KNN Classification on Iris Dataset

## Overview
This project applies **K-Nearest Neighbors (KNN)** classification to the famous **Iris dataset**.  
The workflow includes:
1. Loading and preparing the dataset
2. Normalizing features using **MinMaxScaler**
3. Experimenting with multiple values of K to find the best accuracy
4. Evaluating the best model using accuracy and confusion matrix
5. Visualizing decision boundaries for two selected features

## Files
- `Iris.csv` — Dataset
- `knn_iris.py` — Python script with full implementation
- `confusion_matrix.png` — Heatmap of the confusion matrix
- `decision_boundary.png` — Visualization of the decision boundaries

## Steps Performed
1. **Data Preparation**  
   - Removed the `Id` column  
   - Separated features and target  
   - Normalized features to [0, 1] range

2. **Model Training**  
   - Tested K values from 1 to 20  
   - Chose the best K based on test accuracy

3. **Evaluation**  
   - Accuracy score  
   - Confusion matrix (visualized as heatmap)

4. **Visualization**  
   - Decision boundary plot for `PetalLengthCm` and `PetalWidthCm`

## Dependencies
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
