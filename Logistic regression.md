## Accuracy
- **Core Idea**: Measures the overall correctness of the model.
- **Details**: It is the ratio of correct predictions (both true positives and true negatives) to the total number of cases examined.
- **Formula**: $ \text{Accuracy} = \frac{\text{True Positives} + \text{True Negatives}}{\text{Total Population}} $
- **Library/Function**: `from sklearn.metrics import accuracy_score`

## Precision
- **Core Idea**: Measures the accuracy of positive predictions.
- **Details**: It reflects the proportion of positive identifications that were actually correct.
- **Formula**: $ \text{Precision} = \frac{\text{True Positives}}{\text{True Positives} + \text{False Positives}} $
- **Library/Function**: `from sklearn.metrics import precision_score`

## Recall (Sensitivity)
- **Core Idea**: Measures the ability of a model to find all the relevant cases (True Positives).
- **Details**: It reflects the proportion of actual positives that were identified correctly.
- **Formula**: $ \text{Recall} = \frac{\text{True Positives}}{\text{True Positives} + \text{False Negatives}} $
- **Library/Function**: `from sklearn.metrics import recall_score`

## AUC (Area Under The Curve)
- **Core Idea**: Measures the ability of a classifier to distinguish between classes.
- **Details**: Higher AUC indicates a better performing model, irrespective of the classification threshold.
- **Formula**: No simple formula, as it involves plotting TPR vs. FPR at various threshold settings.
- **Library/Function**: `from sklearn.metrics import roc_auc_score`

## ROC Curve (Receiver Operating Characteristic Curve)
- **Core Idea**: A plot that illustrates the diagnostic ability of a binary classifier system.
- **Details**: It plots the true positive rate (Recall) against the false positive rate at various threshold settings.
- **Formula**: Plot of $ \text{TPR} = \frac{\text{TP}}{\text{TP} + \text{FN}} $ against $ \text{FPR} = \frac{\text{FP}}{\text{TN} + \text{FP}} $
- **Library/Function**: `from sklearn.metrics import roc_curve; matplotlib.pyplot as plt`

## Heatmap (for Confusion Matrix)
- **Core Idea**: Visual representation of the confusion matrix.
- **Details**: Provides a color-coded visualization of the different categories of the confusion matrix, helping in quick assessment.
- **Library/Function**: `import seaborn as sns; sns.heatmap(confusion_matrix, annot=True)`

## Confusion Matrix
- **Core Idea**: Table that describes the performance of a classification model.
- **Details**: Shows actual values vs. predicted values and helps identify misclassifications.
- **Formula**: Consists of four outcomes - True Positive (TP), True Negative (TN), False Positive (FP), and False Negative (FN).
- **Library/Function**: `from sklearn.metrics import confusion_matrix`
