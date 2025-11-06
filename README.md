A Python project leveraging health-record data to predict diabetes, stroke, and coronary heart disease.

Key Features

Binary classification (Logistic Regression & Random Forest) for each disease.

Feature-selection via correlation matrix & mutual information.

Multi-class model detecting which disease a patient may have.

Clean, modular code – easy to understand and extend.


Modeling Approach

Feature Selection

Computed correlation matrix to identify and drop highly correlated features.

Applied mutual information to estimate the relevance of each feature to the target disease.

Selected top features for modeling to reduce dimensionality, over-fitting risk, and improve interpretability.

Binary Classification

Models used:

Logistic Regression — as a baseline, interpretable model.

Random Forest — for capturing non-linear relationships and feature importance.

Workflow: preprocessing → feature selection → train/test split → fit model → evaluate via accuracy, ROC-AUC, confusion matrix.

Multi-Class Classification

Extended the binary setup to classify among multiple disease categories (e.g., none, diabetes, stroke, CHD).

Used the same feature-selection workflow and applied a multi-class variant of Random Forest or another multi-class capable algorithm.
