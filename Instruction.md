Use 'Titanic' dataset

Target: 'alive'

- Pre-processing scheme:
  * Drop feature 'decks'
  * Fill in the missing value 'age' with a simple imputer median
  * Fill in the missing value 'embark' town with simple imputer mode
  * One hot encoding: 'sex', 'embark town', 'alone'
  * Ordinal encoding: 'class'

- Split data to 80:20 with random_state = 0.
- Determine the appropriate evaluation metrics for the Titanic case.
- Choose the best model with cross-validation (n_splits=5):
    * Logistic regression: solver = liblinear
    * KNN: n_neighbors = 3
    * Decision tree: max depth = 3

- Interpret the results of the selected metric.