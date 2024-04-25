
## Accuracy
- **Core Idea**: Measures the overall correctness of the model.
- **Formula**: $\( \text{Accuracy} = \frac{\text{Number of Correct Predictions}}{\text{Total Number of Predictions}} \)$
- **Library/Function**: `scikit-learn` - `from sklearn.metrics import accuracy_score`

## Precision
- **Core Idea**: The ratio of correctly predicted positive observations to the total predicted positives.
- **Formula**: $\( \text{Precision} = \frac{\text{True Positives}}{\text{True Positives + False Positives}} \)$
- **Library/Function**: `scikit-learn` - `from sklearn.metrics import precision_score`

## Recall (Sensitivity)
- **Core Idea**: The ratio of correctly predicted positive observations to all actual positives.
- **Formula**: $\( \text{Recall} = \frac{\text{True Positives}}{\text{True Positives + False Negatives}} \)$
- **Library/Function**: `scikit-learn` - `from sklearn.metrics import recall_score`

## AUC (Area Under Curve)
- **Core Idea**: Represents degree or measure of separability between classes.
- **Library/Function**: `scikit-learn` - `from sklearn.metrics import roc_auc_score`

## ROC (Receiver Operating Characteristic) Curve
- **Core Idea**: Graphical representation of the diagnostic ability of a binary classifier.
- **Library/Function**: `scikit-learn` - `from sklearn.metrics import roc_curve; import matplotlib.pyplot as plt`

## Heatmap (of Confusion Matrix)
- **Core Idea**: Visual representation of the confusion matrix to show the accuracy of predictions.
- **Library/Function**: `seaborn` for plotting - `import seaborn as sns; sns.heatmap(data)`

## Confusion Matrix
- **Core Idea**: Summary of prediction results on a classification problem.
- **Formula**: Matrix with four quadrants: True Positives, True Negatives, False Positives, False Negatives.
- **Library/Function**: `scikit-learn` - `from sklearn.metrics import confusion_matrix`

