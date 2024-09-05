
# Detecting Early Alzheimer's Disease with Machine Learning

This project uses machine learning techniques to detect early signs of Alzheimer's disease from medical data, including 3D MRI scans. The goal is to explore various machine learning models and assess their performance in identifying early Alzheimer's indicators.

## Project Overview

Alzheimer's disease is a progressive neurodegenerative disorder that affects memory and cognitive function. Early detection of Alzheimer's is crucial for timely intervention. This project leverages a dataset containing MRI scans to build models capable of distinguishing early Alzheimer's patients from healthy individuals.

### Key Features
- **Data Preprocessing**: Handling missing data, scaling features, and preparing MRI data for model training.
- **Model Development**: Applying machine learning models such as Logistic Regression, Support Vector Machines (SVM), and more.
- **Cross-Validation**: Using cross-validation techniques to select the best hyperparameters and models.
- **Performance Metrics**: Evaluating models using accuracy, recall, and AUC (Area Under the Curve) metrics.

## Datasets

The dataset used in this project contains 3D MRI scans from Alzheimer's and healthy subjects. The scans are processed and utilized in various machine learning models to predict Alzheimer's disease.

### Data Source
The dataset is sourced from publicly available medical image repositories. Key references used in this project include:
- OASIS Brain Database
- [NeuroImage: 1053-8119](https://doi.org/10.1016/j.neuroimage.2014.10.002)
- Additional datasets referenced in related literature.

## Models and Techniques

### Logistic Regression
- A classification model was used with imputation and without imputation of missing values.
- Hyperparameter tuning using grid search was performed for the regularization parameter.

### Support Vector Machine (SVM)
- SVM models were trained with different kernel types (`rbf`, `linear`, `poly`, `sigmoid`) and hyperparameters (`C`, `gamma`).
- Cross-validation was used to find the best parameter combinations.

## Results

The results show that models with imputation generally outperformed models without imputation. Logistic regression and SVM models were both evaluated using cross-validation to select the best-performing models.

## Installation and Requirements

To run the notebook and experiments locally, you will need the following Python libraries:

- `numpy`
- `pandas`
- `scikit-learn`
- `matplotlib`
- `seaborn`
- `jupyter`

Install the required dependencies with the following command:

```bash
pip install -r requirements.txt
```

## Running the Notebook

To run the notebook, use the following command:

```bash
jupyter notebook detecting-early-alzheimer-s.ipynb
```

## References

1. [Zhang et al., NeuroImage (2014)](https://doi.org/10.1016/j.neuroimage.2014.10.002)
2. [Magnin et al., Neuroradiology (2009)](https://doi.org/10.1007/s00234-008-0463-x)
3. [Ye et al., PRNI (2011)](https://doi.org/10.1109/PRNI.2011.12)
4. [Filipovych & Davatzikos, NeuroImage (2010)](https://doi.org/10.1016/j.neuroimage.2010.12.066)

## License

This project is licensed under the MIT License - see the LICENSE file for details.
