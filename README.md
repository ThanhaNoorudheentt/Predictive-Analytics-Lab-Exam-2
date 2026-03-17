# Predictive-Analytics-Lab-Exam-2
Predictive Analytics Lab Exam-2

# Objective

The objective of this lab exam is to perform a binary classification task. The goal is to analyze the dataset, build a classification model, visualize decision boundaries, and evaluate model performance.

# Exploratory Data Analysis (EDA)

Dataset:
* The dataset consists of 1020 entries
* Features:

  * `Feature1` 
  * `Feature2` 
* Target:

  * `Target` (binary: Yes/No → encoded as 1/0)
  
# Data Preprocessing

* Converted categorical target values (`Yes`, `No`) into numerical format (`1`, `0`)
* Removed rows with missing target values (20 rows)
* Identified and removed outliers in `Feature1`
* Applied **StandardScaler** to normalize feature values


### Key Observations:

* No missing values in features; some missing values in target were handled
* Class distribution is slightly imbalanced
* Scatter plot shows that:

  * Class 1 points are concentrated in the center
  * Class 0 points are more spread out
* Data is **not linearly separable**

---

# Models Used:

1. Logistic Regression

* Used as a baseline model
* Assumes a **linear decision boundary**
*  Accuracy 0.79


2. Decision Tree Classifier 

* Captures **non-linear relationships**
* Provides flexible decision boundaries
* Better suited for this dataset
* Accuracy 0.96

# Decision Boundary Visualization

* Decision boundary plotted using both models

# Model Evaluation

### 🔹 Decision Tree Results:

* **Accuracy:** 0.96

### 🔹 Confusion Matrix:

```
[[152   6]
 [  2  40]]
```

### 🔹 Classification Report:

* Class 0:

  * Precision: 0.99
  * Recall: 0.96
  * F1-score: 0.97
* Class 1:

  * Precision: 0.87
  * Recall: 0.95
  * F1-score: 0.91

---

# Error Analysis

* The model performs very well with **high accuracy (96%)**

# Observations

* Logistic Regression underperformed due to **linear assumptions**
* Decision Tree handled **non-linearity effectively**
* Feature scaling improved model stability
* Outlier removal improved visualization and model learning

# Conclusion

* The **Decision Tree model outperformed Logistic Regression**
* Achieved **high accuracy with minimal errors**
* Suitable for datasets with **non-linear patterns**

# Tools & Libraries Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

# How to Run

1. Open the notebook
2. Upload the dataset (`Lab_Exam_binary_classification_dataset.csv`)
3. Run all cells sequentially
4. View outputs including:

   * EDA plots
   * Decision boundary
   * Model evaluation

**Thanha Noorudheen**
** Roll no: 253135 **
