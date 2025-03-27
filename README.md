# Wine Quality Classification with Logistic Regression and Regularization

This notebook explores the use of logistic regression with L1 (Lasso) and L2 (Ridge) regularization techniques to classify wine quality based on physicochemical features.

## Objective

To evaluate how regularization impacts model performance and feature importance when predicting whether a wine sample is of good or bad quality.

## Dataset

- **Source**: UCI Machine Learning Repository
- **Dataset**: Wine Quality Dataset
- **Target**: Binary classification – Good (quality >= 7) vs Bad (quality < 7)

## Key Steps

1. **Data Preprocessing**
   - Loaded and inspected the dataset
   - Converted multi-class quality scores into binary classes

2. **Train-Test Split**
   - Split the dataset into training and test sets using `train_test_split`

3. **Modeling with Logistic Regression**
   - Applied logistic regression with:
     - No regularization (baseline)
     - L1 regularization (Lasso)
     - L2 regularization (Ridge)


4. **Model Evaluation**
   - Evaluated models using:
     - Accuracy
     - Confusion Matrix
     - Classification Report
   - Analyzed and compared the effect of different regularization types

5. **Feature Importance**
   - Visualized feature coefficients to understand which features were most influential

## Dependencies

- Python
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## Results Summary

- L1 regularization helped in feature selection by reducing coefficients of less important features to zero
- L2 regularization retained all features but penalized large coefficients
- Regularization improved generalization and mitigated overfitting

## Conclusion

Regularization techniques are useful tools to improve model interpretability and avoid overfitting, especially in high-dimensional or noisy datasets.

## License

This project is licensed under the MIT License.

The Wine dataset used is from the UCI Machine Learning Repository and is in the **public domain**.  
Reference: https://archive.ics.uci.edu/ml/datasets/Wine

