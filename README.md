# Tumor-Cell-Analysis-Project
This project analyzes tumor cell data from 550 patients using Python. It involves data cleaning, exploratory analysis, feature engineering, and machine learning to classify tumors as malignant or benign. Techniques include PCA, logistic regression, and k-fold cross-validation to ensure model accuracy and reliability.

# Tumor Cell Analysis Project

## Description
This project analyzes tumor cell data from 550 patients using Python. It involves data cleaning, exploratory analysis, feature engineering, and machine learning to classify tumors as malignant or benign. Techniques include PCA, logistic regression, and k-fold cross-validation to ensure model accuracy and reliability.

## Table of Contents
- [Description](#description)
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Data Description](#data-description)
- [Analysis and Results](#analysis-and-results)
- [Modeling](#modeling)
- [Conclusion](#conclusion)
- [Contributing](#contributing)

* NOTE: TO QUICKLY VIEW PROJECT CONTENTS, OPEN THE PDF FILE !!! 

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/Hashezm/tumor-cell-analysis.git
    ```
2. Navigate to the project directory:
    ```bash
    cd tumor-cell-analysis
    ```
3. Install the necessary packages:
    ```bash
    pip install -r requirements.txt
    ```

## Usage
1. Open the Jupyter notebook:
    ```bash
    jupyter notebook Tumor-Cell-Analysis-Project.ipynb
    ```
2. Execute the cells in the notebook to load the data, perform analysis, and build the models.

## Features
- **Data Loading and Cleaning**: Loading the dataset, checking for missing values, and performing data imputation.
- **Exploratory Data Analysis**: Generating summary statistics and visualizing correlations between features.
- **Label Encoding**: Encoding the diagnosis column to numerical values.
- **Data Partitioning**: Splitting the data into training and testing sets.
- **Standardization**: Standardizing the features.
- **Principal Component Analysis (PCA)**: Reducing the number of features.
- **Logistic Regression Model**: Building and evaluating a logistic regression model.
- **Cross-Validation**: Performing k-fold cross-validation.
- **Final Validation and Prediction**: Testing the model on a test set and making predictions on new data.

## Data Description
The dataset consists of the following columns:
1. `patient_id`: Unique identifier for each patient.
2. `diagnosis`: Diagnosis of the tumor cells (M = malignant, B = benign).
3. `feature_1` to `feature_30`: Numerical features representing various properties of the tumor cells.

The data is located in the file `/public/bmort/python/tumor_cells.csv`.

## Analysis and Results
### Data Loading and Cleaning
- Loaded the dataset into a DataFrame.
- Checked for missing values and performed necessary imputations.

### Summary Statistics
- Generated summary statistics for each feature.
- Identified and handled outliers.
- Compared ranges and magnitudes of the features.

### Correlation Heatmap
- Used Seaborn's `heatmap()` function to visualize correlations between features.

### Label Encoding
- Encoded the `diagnosis` column with 0 for benign and 1 for malignant.

### Data Partitioning
- Split the dataset into 80% training and 20% testing sets.

### Standardization
- Standardized the features to have a mean of 0 and a standard deviation of 1.

### Principal Component Analysis (PCA)
- Applied PCA to reduce the number of features.
- Selected the number of components based on explained variance.

### Logistic Regression Model
- Built a logistic regression model using the PCA-transformed features.
- Evaluated the model using k-fold cross-validation.

### Final Validation
- Tested the model on the test set.
- Generated a confusion matrix and calculated accuracy.

### Prediction for New Patient
- Loaded new patient data from `/public/bmort/python/new_patient.pkl`.
- Predicted the diagnosis using the logistic regression model.

## Conclusion
Summarized the findings from the analysis and modeling. Provided insights into the classification performance and the effectiveness of PCA in feature reduction.

## Contributing
Contributions are welcome! Please submit a pull request or open an issue to discuss your ideas.


