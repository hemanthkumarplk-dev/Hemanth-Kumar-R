# Decision Trees and Random Forests

## 📌 Objective

The goal of this task was to **learn tree-based models for classification** and evaluate them using the Heart Disease dataset.

---

## 🛠 Tools Used

* **Python**
* **Scikit-learn** (DecisionTree, RandomForest, Cross-validation)
* **Matplotlib / Seaborn** (Visualization)

---

## 🚀 Steps Completed

### 1. Train a Decision Tree Classifier and Visualize

* Built a **Decision Tree Classifier** on the dataset.
* Used `plot_tree` to **visualize the tree structure**.
* Showed how the model makes splits and predictions.

### 2. Analyze Overfitting and Control Tree Depth

* Trained a **full-depth tree** → observed high training accuracy but lower test accuracy (overfitting).
* Trained a **pruned tree** with `max_depth=4` → reduced complexity, better generalization.

### 3. Train a Random Forest and Compare Accuracy

* Built a **Random Forest Classifier** with 100 trees.
* Compared its accuracy against the Decision Tree.
* Random Forest gave **higher accuracy and better stability**.

### 4. Interpret Feature Importances

* Extracted **feature importances** from the Random Forest.
* Plotted a bar chart ranking features (most important to least important).
* Helped in understanding which attributes strongly influence predictions.

### 5. Evaluate using Cross-Validation

* Performed **5-fold cross-validation** for both Decision Tree and Random Forest.
* Reported **average accuracy scores**, ensuring more robust evaluation.

---

## 📊 Key Learnings

* **Decision Trees** are easy to interpret but prone to overfitting.
* **Pruning (max_depth, min_samples_split, etc.)** helps improve generalization.
* **Random Forests** reduce overfitting by combining multiple trees (bagging).
* **Feature Importances** provide interpretability of model decisions.
* **Cross-validation** ensures performance is not dataset-split dependent.


