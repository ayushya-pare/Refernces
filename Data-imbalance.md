
# Data Imbalance

## Data Imbalance
- **Issue**: Occurs when classes in the target variable are unequally represented.
- **Impact**: Can bias the prediction model towards the majority class.

## Techniques for Handling Data Imbalance
- **Upsampling**: Increasing the number of instances in the minority class by duplication.
- **Downsampling**: Decreasing the number of instances in the majority class.

## Libraries and Functions
- Python libraries: `sklearn`, `imbalanced-learn`
- Functions: `SMOTE()`, `resample()`

## Example Code
```python
from sklearn.linear_model import LogisticRegression
from imblearn.over_sampling import SMOTE
# example setup code
# Handling imbalance
smote = SMOTE(random_state=42)
X_resampled, y_resampled = smote.fit_resample(X_train, y_train)

# Training logistic regression
model = LogisticRegression()
model.fit(X_resampled, y_resampled)

# Predicting
predictions = model.predict(X_test)


