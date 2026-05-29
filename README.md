# Alzheimer's Disease Detection using Machine Learning

## Project Overview

This project implements a machine learning model to detect and classify Alzheimer's disease stages using clinical data. The model leverages diagnostic information, cognitive scores, and biomarker data to provide accurate disease classification.

## Objective

The goal of this project is to:
- Build a predictive model for Alzheimer's disease classification
- Process and merge multi-source clinical datasets
- Standardize and encode features for machine learning
- Train a Random Forest Classifier for accurate diagnosis prediction

## Dataset

The project uses clinical data containing:
- **Diagnosis Target**: Actual diagnoses of patients
- **Cognitive Scores**: Cognitive assessment results
- **Biomarkers & Data**: Clinical measurements and imaging data (FDG-PET, etc.)

The data is merged on patient identifiers (RID) to create a comprehensive feature set.

## Disease Classification

The model predicts three categories:
- **CN**: Cognitively Normal
- **LMCI**: Late Mild Cognitive Impairment  
- **AD**: Alzheimer's Disease

## Technologies & Libraries

- **Python 3.x**
- **pandas**: Data manipulation and merging
- **numpy**: Numerical computations
- **scikit-learn**: Machine learning algorithms
  - StandardScaler: Feature scaling
  - train_test_split: Data splitting
  - RandomForestClassifier: Classification model
  - LabelEncoder: Categorical encoding
- **matplotlib**: Data visualization
- **openpyxl**: Excel file handling

## Project Workflow

1. **Data Loading**: Load multiple sheets from Excel file
2. **Data Cleaning**: Remove missing values
3. **Data Integration**: Merge datasets on patient ID
4. **Feature Scaling**: Standardize numerical features
5. **Feature Engineering**: Encode categorical variables
6. **Model Training**: Train Random Forest Classifier
7. **Evaluation**: Assess model performance

## Key Features

- Multi-sheet Excel data integration
- Automatic handling of missing values
- Standardized feature scaling
- Categorical variable encoding
- Train-test split (80-20)
- Random Forest ensemble learning

## Usage

```python
# Load the notebook and run cells sequentially
# Ensure the data file "CSI_7_MAL_2324_CW_resit_data.xlsx" is in the same directory

# The notebook will:
# 1. Load and merge clinical datasets
# 2. Preprocess the data
# 3. Train the model
# 4. Generate predictions
```

## Files

- `Alzheimer's Detection.ipynb` - Main Jupyter notebook with complete pipeline
- `CSI_7_MAL_2324_CW_resit_data.xlsx` - Clinical dataset (required)

## Model Details

- **Algorithm**: Random Forest Classifier
- **Train-Test Split**: 80-20
- **Feature Scaling**: StandardScaler
- **Encoding**: LabelEncoder for target variable

## Model Performance Metrics

The model's performance can be evaluated using:
- Accuracy
- Precision & Recall
- Confusion Matrix
- Classification Report

## Learning Outcomes

This project demonstrates:
- Data preprocessing and integration
- Feature engineering techniques
- Model training and validation
- Medical data analysis
- Machine learning best practices

## Future Enhancements

- Feature importance analysis
- Hyperparameter tuning
- Cross-validation implementation
- Additional classification algorithms comparison
- Model interpretability with SHAP values
- Web interface for predictions

## License

This project is part of my Machine Learning Projects collection.

## Author

Mohamed Diaby Gassama
---

**Note**: This project requires the clinical dataset to run. Ensure all dependencies are installed before execution.
