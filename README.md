# Titanic Survival Prediction & Analysis 🚢

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Scikit-Learn](https://img.shields.io/badge/Machine%20Learning-Scikit--Learn-orange.svg)](https://scikit-learn.org/)

A comprehensive end-to-end data science project focused on predicting passenger survival on the Titanic. This repository includes exploratory data analysis (EDA), feature engineering, and a comparison of multiple machine learning models with hyperparameter optimization.

## 📊 Project Overview

This project analyzes the famous Titanic dataset to identify key factors that influenced survival rates. By applying data cleaning, visualization, and machine learning techniques, we developed a model capable of predicting survival outcomes with approximately **83% accuracy**.

### Key Findings
- **Gender & Class:** Female passengers and those in 1st class had significantly higher survival rates.
- **Wealth Factor:** Passengers who paid higher fares were more likely to survive.
- **Family Size:** Travelling with small to medium-sized families showed different survival patterns compared to solo travellers.

## 🛠️ Features

- **Data Preprocessing:** Handled missing values (Age, Cabin, Embarked) and categorical encoding.
- **Feature Engineering:** Created `FamilySize` to capture family-related survival patterns.
- **Exploratory Data Analysis:** 
    - Statistical summaries.
    - Correlation heatmaps.
    - Interactive visualizations using **Plotly**.
- **Machine Learning Models:**
    - K-Nearest Neighbors (KNN)
    - Decision Tree Classifier
    - Random Forest Classifier (Best Performer)
- **Model Optimization:** Hyperparameter tuning using `RandomizedSearchCV`.

## 📁 Repository Structure

```bash
|
├── docs/               # Project documentation and detailed reports
│   └── analysis_report.md
├── notebooks/          # Jupyter notebooks for analysis and modeling
│   └── titanic_analysis.ipynb
├── LICENSE             # MIT License
├── requirements.txt    # Project dependencies
└── README.md           # Project documentation
```

## 🚀 Getting Started

### Prerequisites
- Python 3.8 or higher
- Jupyter Notebook or JupyterLab

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/titanic-analysis.git
   cd titanic-analysis
   ```

2. **Create a virtual environment (optional but recommended):**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

### Data Acquisition

The dataset used in this project is the Titanic dataset from Kaggle.
1. Download `train.csv` from [Kaggle Titanic Competition](https://www.kaggle.com/c/titanic/data).
2. Place the `train.csv` file in the `data/` directory.

### Running the Analysis

1. Launch Jupyter Notebook from the root directory:
   ```bash
   jupyter notebook
   ```
2. Navigate to `notebooks/titanic_analysis.ipynb`.
3. **Note:** If running the notebook from the `notebooks/` directory, ensure the data path in the loading cell points to `../data/train.csv`.

## 📈 Results

| Model | Accuracy | F1-Score |
| :--- | :---: | :---: |
| KNN (Tuned) | ~76% | ~0.69 |
| Decision Tree (Tuned) | ~79% | ~0.74 |
| **Random Forest (Tuned)** | **~83%** | **~0.79** |

For a more detailed breakdown of the methodology and results, please refer to the [Full Analysis Report](docs/analysis_report.md).

## 📄 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing
Contributions are welcome! If you have suggestions for improving the model or the analysis, feel free to open an issue or submit a pull request.

---
*Created as part of the Py-and-AI Bootcamp.*
