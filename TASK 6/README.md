# K-Nearest Neighbors (KNN) Classification on Iris Dataset

## 📌 Project Overview

This project demonstrates how to implement **K-Nearest Neighbors (KNN)** for classification using the famous **Iris dataset**.
We followed a step-by-step workflow to load data, preprocess it, train a KNN model, evaluate performance, and visualize decision boundaries.

---

## 🚀 Steps Followed

### 1. Load and Preprocess Dataset

* Loaded the **Iris dataset** (`Iris.csv`).
* Removed the unnecessary `Id` column.
* Separated features (`SepalLengthCm`, `SepalWidthCm`, `PetalLengthCm`, `PetalWidthCm`) and target (`Species`).
* Normalized features using **StandardScaler** to ensure fair distance measurement for KNN.

### 2. Train/Test Split

* Split the dataset into **training (80%)** and **testing (20%)** sets using `train_test_split`.
* Used stratified sampling to maintain class balance across splits.

### 3. Train KNN Classifier

* Implemented `KNeighborsClassifier` from **scikit-learn**.
* Trained models with different **values of K (1, 3, 5, 7, 9, 11)**.
* Compared accuracies for each value of K.

### 4. Model Evaluation

* Chose the best-performing K.
* Evaluated model using:

  * **Accuracy Score**
  * **Confusion Matrix** (visualized with heatmap)

### 5. Visualize Decision Boundaries

* Used only the first two features (Sepal length & Sepal width) for 2D visualization.
* Plotted decision regions created by KNN to show how classes are separated.
* Encoded categorical labels into integers for proper visualization.

---

## 🛠 Tools & Libraries Used

* **Pandas** – Data loading & preprocessing
* **NumPy** – Numerical operations
* **Scikit-learn** – KNN model, preprocessing, evaluation
* **Matplotlib** – Visualization

---

## 📊 Results

* KNN achieved high accuracy on the Iris dataset (varies depending on K).
* Confusion matrix showed correct classification across most classes.
* Decision boundary visualization provided insight into how KNN separates classes in feature space.

---

## 📂 Files

* `Iris.csv` → Dataset file
* `knn_classification.py` → Python code implementing all steps

---

## ✅ Conclusion

KNN is a simple yet powerful algorithm for classification.
With normalized features and a suitable K value, it performs very well on the **Iris dataset**, making it an excellent introduction to supervised classification tasks.
