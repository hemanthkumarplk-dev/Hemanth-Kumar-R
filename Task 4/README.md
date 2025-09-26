# Logistic Regression Workflow

## 1. Choose a binary classification dataset

-   Used the **Breast Cancer Wisconsin Diagnostic dataset**
    (`data(1).csv`).
-   Target variable: `diagnosis`
    -   Encoded as **M = 1 (Malignant)**, **B = 0 (Benign)**.
-   Removed irrelevant columns (`id`, `Unnamed: 32`).

## 2. Train/test split and standardize features

-   Split data into **80% training** and **20% testing** sets using
    `train_test_split`.
-   Standardized features with `StandardScaler` to ensure each has mean
    = 0 and variance = 1 (important for Logistic Regression).

## 3. Fit a Logistic Regression model

-   Trained logistic regression with
    `LogisticRegression(max_iter=10000)`.
-   Model learns weights (coefficients) for each feature to estimate
    probability of being malignant.

## 4. Evaluate model performance

-   **Confusion Matrix** → shows true positives, true negatives, false
    positives, and false negatives.
-   **Precision** → of the samples predicted malignant, how many were
    actually malignant.
-   **Recall (Sensitivity)** → of the malignant samples, how many were
    correctly identified.
-   **ROC-AUC** → measures overall ability of the model to distinguish
    between classes.
-   Plotted **ROC Curve** to visualize trade-off between true positive
    rate and false positive rate.

## 5. Tune threshold and explain sigmoid function

-   By default, logistic regression uses a threshold of **0.5**.
-   You experimented with lowering/raising the threshold (e.g., 0.4,
    0.7) to balance **precision vs recall**.
-   Logistic regression uses the **sigmoid function**:

\[ `\sigma`{=tex}(z) = `\frac{1}{1 + e^{-z}}`{=tex} \]

-   It converts the linear model output into a probability between **0
    and 1**.
-   Thresholding this probability determines the final class prediction.


