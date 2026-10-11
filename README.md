# Breast Cancer Classification with Machine Learning

An end-to-end machine learning project for classifying breast tumors as **malignant** or **benign** using the Breast Cancer Wisconsin (Diagnostic) dataset.

This project demonstrates a complete machine learning workflow, including exploratory data analysis, preprocessing, model comparison, hyperparameter tuning, evaluation, and interpretation.

> **Disclaimer:** This project is intended for educational and research purposes only. It is not a medical device and must not be used for diagnosis or medical decisions.

##  Available Languages

This repository includes two versions of the Jupyter Notebook, allowing users to explore the project in their preferred language.

- 🇬🇧 **English version:** `breast-cancer-classification.ipynb`
- 🇫🇷 **French version:** `breast-cancer-classification-fr.ipynb`

Both notebooks cover the same project and machine learning workflow. The main difference is the language used for explanations, documentation, and analysis.

Choose the notebook that best suits your language preference.

##  Project Overview

The objective is to build and evaluate machine learning models capable of distinguishing between malignant and benign breast tumors based on numerical diagnostic features.

The project focuses on developing a reproducible workflow while applying good practices in data preprocessing, model validation, and performance evaluation.

### Key Features

- Dataset inspection and data quality analysis
- Exploratory Data Analysis (EDA)
- Class distribution and feature visualization
- Feature correlation analysis
- Data preprocessing and scaling
- Train/test splitting to help prevent data leakage
- Machine learning pipelines
- Stratified cross-validation
- Comparison of baseline and machine learning models
- Hyperparameter tuning
- Final evaluation on a held-out test set
- Confusion matrix and classification metrics
- ROC curve and Precision-Recall analysis
- Error analysis
- Permutation feature importance
- Unsupervised learning exploration using clustering and PCA

##  Dataset

The project uses the **Breast Cancer Wisconsin (Diagnostic)** dataset, available directly through `scikit-learn`.

Dataset characteristics:

- **569 samples**
- **30 numerical features**
- **2 target classes:** malignant and benign
- No separate dataset download is required

The features describe characteristics of cell nuclei computed from digitized images of breast masses.

For cancer-focused evaluation, the target is explicitly encoded as:

- `1` — Malignant
- `0` — Benign

This encoding makes it easier to interpret recall, precision, and other classification metrics with malignant cases as the positive class.

##  Technologies Used

- **Python**
- **Jupyter Notebook**
- **NumPy**
- **Pandas**
- **Matplotlib**
- **Seaborn**
- **Scikit-learn**

##  Repository Structure

```text
breast-cancer-classification/
│
├── breast-cancer-classification.ipynb
├── breast-cancer-classification-fr.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

**Notebook descriptions:**

- `breast-cancer-classification.ipynb`: English documentation and analysis.
- `breast-cancer-classification-fr.ipynb`: French documentation and analysis.

##  Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/breast-cancer-classification.git
cd breast-cancer-classification
```

Replace `YOUR-USERNAME` with your GitHub username.

### 2. Create a virtual environment

**Windows (PowerShell):**

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
```

**macOS / Linux:**

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Install the dependencies

```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open either notebook:

- `breast-cancer-classification.ipynb` for the English version.
- `breast-cancer-classification-fr.ipynb` for the French version.

Run the notebook cells sequentially to reproduce the analysis, train the models, and generate the visualizations.

You can also use JupyterLab or Visual Studio Code.

##  Machine Learning Workflow

The project follows these main steps:

1. **Data loading and inspection:** load the dataset and examine its structure, features, and target classes.
2. **Exploratory analysis:** investigate distributions, correlations, and potential patterns.
3. **Data preparation:** split the dataset into training and test sets before fitting preprocessing transformations.
4. **Pipeline construction:** combine preprocessing and model training to reduce the risk of data leakage.
5. **Model comparison:** evaluate multiple classifiers using stratified cross-validation.
6. **Hyperparameter tuning:** optimize selected models using training data.
7. **Final evaluation:** assess the selected model on the held-out test set.
8. **Model interpretation:** examine errors and permutation feature importance.
9. **Additional exploration:** investigate the dataset using clustering and Principal Component Analysis (PCA).

##  Evaluation Metrics

The project uses several complementary metrics to assess model performance.

| Metric | Description |
|---|---|
| Malignant Recall | Proportion of malignant cases correctly identified |
| Malignant Precision | Proportion of predicted malignant cases that are truly malignant |
| Malignant F1-score | Harmonic mean of malignant precision and recall |
| ROC-AUC | Measures how well the model ranks positive and negative cases |
| Average Precision | Summarizes the precision-recall curve |
| Balanced Accuracy | Average recall across both classes |
| Confusion Matrix | Shows correct and incorrect predictions for each class |

No single metric is sufficient to establish clinical usefulness. In particular, false negatives and false positives have different implications and must be considered carefully.

Run the notebooks in your own environment to reproduce the results and visualizations. Results may vary depending on software versions, model settings, and execution details.

##  Limitations

- The dataset is relatively small and comes from a single source.
- The models have not been externally validated on independent hospitals or populations.
- The input consists of structured numerical measurements, not raw medical images such as MRI scans or mammograms.
- The default classification threshold may not be appropriate for every application.
- Subgroup representativeness and fairness have not been established.
- Feature importance describes model behavior; it does not establish causality or clinical evidence.
- High performance on this dataset does not guarantee reliable performance in real-world clinical settings.

This project is a machine learning learning exercise and should not be interpreted as a validated medical diagnostic system.

##  Possible Future Improvements

- Evaluate additional classification algorithms.
- Explore alternative threshold-selection strategies.
- Add calibration analysis.
- Perform external validation on independent datasets.
- Investigate subgroup performance and fairness.
- Improve experiment tracking and reproducibility.
- Package the selected model in a simple demonstration application.



Master's student in Artificial Intelligence, interested in machine learning, data science, and intelligent systems.

##  References

- Wolberg, W. H., Street, W. N., & Mangasarian, O. L. — Breast Cancer Wisconsin (Diagnostic) dataset.
- Scikit-learn documentation: [Breast cancer Wisconsin dataset](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_breast_cancer.html)
- Scikit-learn documentation: [Pipelines and composite estimators](https://scikit-learn.org/stable/modules/compose.html)
- Scikit-learn documentation: [Model evaluation](https://scikit-learn.org/stable/modules/model_evaluation.html)

---

*Built for learning, experimentation, and exploration of machine learning techniques.*
