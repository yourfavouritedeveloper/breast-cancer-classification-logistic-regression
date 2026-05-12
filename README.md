#  Breast Cancer Classification with Logistic Regression

A machine learning project that classifies breast cancer tumors as **benign** or **malignant** using Logistic Regression on the UCI Wisconsin Breast Cancer dataset.

##  Results

| Metric | Score |
|--------|-------|
| Test Accuracy | 95.62% |
| Cross-Validation Accuracy (10-fold) | 96.70% |
| CV Standard Deviation | ±1.97% |

## Project Structure

```
├── breast_cancer.csv        # Dataset (UCI Wisconsin Breast Cancer)
├── main.ipynb               # Main notebook
└── README.md
```

## Pipeline

1. **Data Loading** — Load the UCI Wisconsin Breast Cancer dataset
2. **Preprocessing** — Handle missing values with mean imputation
3. **Train/Test Split** — 80/20 split with `random_state=0`
4. **Feature Scaling** — StandardScaler for normalization
5. **Model Training** — Logistic Regression classifier
6. **Evaluation** — Confusion matrix, accuracy score, and 10-fold cross-validation
7. **Visualization** — PCA-based regression line plot

## Dataset

The [UCI Wisconsin Breast Cancer dataset](https://archive.ics.uci.edu/dataset/15/breast+cancer+wisconsin+original) contains 683 samples with 9 features:

| Feature | Description |
|--------|-------------|
| Clump Thickness | 1–10 |
| Uniformity of Cell Size | 1–10 |
| Uniformity of Cell Shape | 1–10 |
| Marginal Adhesion | 1–10 |
| Single Epithelial Cell Size | 1–10 |
| Bare Nuclei | 1–10 |
| Bland Chromatin | 1–10 |
| Normal Nucleoli | 1–10 |
| Mitoses | 1–10 |

**Target:** `Class` — `2` (Benign) or `4` (Malignant)

## Requirements

```bash
pip install numpy pandas matplotlib scikit-learn
```

## Usage

1. Clone the repo:
```bash
git clone https://github.com/your-username/breast-cancer-classification-logistic-regression.git
cd breast-cancer-classification-logistic-regression
```

2. Add `breast_cancer.csv` to the project directory

3. Open and run the notebook:
```bash
jupyter notebook breast_cancer.ipynb
```

## Visualizations

- **Confusion Matrix** — True vs predicted classifications
- **Actual vs Predicted Plot** — Per-sample prediction comparison
- **PCA Regression Line** — All 9 features compressed to 1D for visualization
