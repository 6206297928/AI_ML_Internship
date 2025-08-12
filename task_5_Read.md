# Heart Disease Prediction with Decision Tree

## Overview
This project trains and analyzes Decision Tree classifiers on the Heart Disease dataset (`heart.csv`).
We:
1. Load and explore the dataset
2. Train an overfitted Decision Tree (no depth limit)
3. Train a pruned Decision Tree (controlled depth)
4. Compare training & testing accuracy to detect overfitting
5. Use cross-validation to find the best `max_depth`
6. Visualize both trees
7. Analyze feature importances

---

## Dataset
The `heart.csv` dataset contains 1025 patient records with features like:
- **age**: Age of the patient
- **sex**: Gender (1 = male, 0 = female)
- **cp**: Chest pain type
- **trestbps**: Resting blood pressure
- **chol**: Serum cholesterol
- **thalach**: Maximum heart rate achieved
- **oldpeak**: ST depression induced by exercise
- ... and more.

Target variable:
- **target**: 1 = disease present, 0 = disease absent

---

## How to Run
```bash
# Activate environment
conda activate internship

# Install dependencies
conda install -n internship numpy pandas matplotlib seaborn scikit-learn graphviz python-graphviz notebook

# Launch Jupyter
jupyter notebook
