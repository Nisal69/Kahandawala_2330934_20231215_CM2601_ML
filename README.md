# Predicting Bank Deposits Using Machine Learning

## Overview
This repository contains a machine learning project aimed at predicting whether a person will make a bank deposit. The analysis is based on the UCI Bank Marketing dataset. The project uses two machine learning models: a Neural Network and a Random Forest Classifier, with the goal of achieving an accuracy of 90% or higher.

## Dataset
- **Size**: 45,211 records
- **Features**: 17 total
  - 9 categorical
  - 8 numerical

### Feature Selection and Dataset Simplification
To improve model performance, the dataset was simplified by removing unnecessary features:
- **`Default`**: Dropped due to most values being "no," making it irrelevant to the outcome.
- **`Pdays`**: Dropped because most values are -1, rendering it ineffective for predictions.

Other preprocessing steps included encoding categorical variables, handling class imbalance, and feature scaling. Details are available in the report.

## Tools and Libraries Used
The following tools and libraries were used for data preprocessing and model implementation:
- **Pandas**: For data manipulation and preprocessing.
- **Matplotlib**: For data visualization.
- **Scikit-learn**: For model building and evaluation.
- **NumPy**: For numerical computations.

## Models Implemented
1. **Neural Network**:
   - Architecture:
     - Input Layer: 17 features
     - Hidden Layer: 128 neurons with ReLU activation and dropout for regularization
     - Output Layer: 1 neuron with Sigmoid activation
   - Achieved accuracy: 91.73% (after applying SMOTE).

2. **Random Forest Classifier**:
   - Hyperparameter Tuning:
     - Number of trees (n\_estimators)
     - Maximum depth
     - Splitting criteria (Gini, entropy)
   - Achieved strong performance in identifying negative cases but requires optimization for reducing false positives.

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/your-repo-name.git](https://github.com/Nisal69/Kahandawala_2330934_20231215_CM2601_ML.git
   ```

## Results
- **Neural Network**:
  - Accuracy: 91.73%
  - Improved performance with SMOTE for class imbalance handling.

- **Random Forest**:
  - Effective for majority class predictions.
  - Requires further tuning for improved recall of minority class.

## Key Observations
- Data preprocessing, including feature selection and balancing, significantly impacted model performance.
- SMOTE effectively handled class imbalance, improving the Neural Network's ability to predict minority class cases.

## Future Work
- Explore alternative balancing techniques such as ADASYN.
- Test ensemble models like XGBoost and LightGBM for improved accuracy.
- Perform additional feature engineering for enhanced insights.

## License
This project is licensed under the MIT License.

## Contact
For any queries or contributions, feel free to contact: [nisalkahandawala@gmail.com].
