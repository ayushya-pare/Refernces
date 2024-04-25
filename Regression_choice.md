                 Is your outcome variable...
                            |
              --------------------------
             |                            |
         Continuous                  Categorical
             |                            |
       ----------------                --------------
      |                |              |             |
    One predictor   Multiple         Binary       Multi-class
      |                |              |             |
     Linear       Multiple         Logistic     classification models
    Regression   Regression       Regression                
                                                    
---------------------------------------------

Numeric Transformer

    Concept: Scales numerical features to have mean 0 and variance 1, which is crucial for many machine learning algorithms.
    
    Formula/Function: $z=(x−μ)σz=σ(x−μ)​$
    Library/Function: Uses StandardScaler() from scikit-learn.preprocessing.
    
    
    from sklearn.preprocessing import StandardScaler\n
    numeric_transformer = Pipeline(steps=[("scaler", StandardScaler())])

Categorical Transformer

    Concept: Converts categorical variables into a format that can be provided to ML algorithms 
    via one-hot encoding.
        Explanation: Transforms each categorical class into a new binary variable (0 or 1).
        Library/Function: Uses OneHotEncoder(handle_unknown="ignore") from scikit-learn.preprocessing to create dummy variables and ignore any unknown categories not seen during training.

Preprocessor

    Concept: Combines transformations for both numerical and categorical data using a ColumnTransformer. This allows different columns or column subsets of the input to be transformed separately.
        Explanation: Applies specified transformers to columns of an array or pandas DataFrame.
        Library/Function: Uses ColumnTransformer() from scikit-learn.compose to apply the specified transformations to the named columns, separating the handling of different feature types.

python

from sklearn.compose import ColumnTransformer
preprocessor = ColumnTransformer(
    transformers=[
        ("num", numeric_transformer, continious_features),
        ("cat", categorical_transformer, categorical_features)
    ]
)



        
