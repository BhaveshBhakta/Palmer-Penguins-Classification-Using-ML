## Palmer Penguins Classification

### Project Overview

This project focuses on classifying **penguin species** from the Palmer Penguins dataset based on various physical measurements such as bill length and depth, flipper length, and body mass, along with the island of observation. The goal is to develop a machine learning model that can accurately distinguish between different penguin species (specifically, Adelie and Gentoo, as this dataset is for binary classification).

-----

### Technical Highlights

  * **Dataset**: [Kaggle - Palmer Penguins for Binary Classification](https://www.kaggle.com/datasets/martaarroyo/palmer-penguins-for-binary-classification)
  * **Size**: 274 entries, 7 columns
  * **Key Features**:
      * island, bill\_length\_mm, bill\_depth\_mm, flipper\_length\_mm, body\_mass\_g, year
  * **Approach**:
      * Data Cleaning: No missing values or duplicates were found.
      * Exploratory Data Analysis: Histograms, Boxplots, and Heatmaps were used for visualization.
      * Label Encoding: Applied to all columns, including numerical ones (as per the notebook) and the target `species`.
      * Data Standardization using `StandardScaler`.
      * Binary Classification: The target variable `species` has two categories: 'Adelie' and 'Gentoo'.
      * Models Used:
          * Logistic Regression, Ridge Classifier, SVC, Random Forest, XGBoost, AdaBoost, Gradient Boosting, Bagging, Decision Tree.
  * **Best Accuracy**:
      * 100% across all models (Logistic Regression, Ridge Classifier, XGBoost, Random Forest, AdaBoost, Gradient Boosting, Bagging, Decision Tree, SVC). This extremely high accuracy might indicate that the two species are very distinct based on the provided features, or potentially a form of data leakage.

-----

### Purpose and Applications

  * Automate the **identification of penguin species** in ecological studies.
  * Aid researchers in analyzing population dynamics and environmental impacts on penguin colonies.
  * Serve as a valuable tool for educational purposes in biology and data science.
  * Demonstrate the effectiveness of machine learning in ecological classification tasks.

-----

### Installation

Clone the repository:

```bash
git clone https://github.com/BhaveshBhakta/Palmer-Penguins-Classification-Using-ML.git
cd Palmer-Penguins-Classification-Using-ML
```

Install the necessary libraries:

```bash
pip install pandas numpy seaborn matplotlib scikit-learn xgboost
```

-----

### Collaboration

We welcome contributions to improve the project. You can help by:

  * Investigating the source of the 100% accuracy to ensure no data leakage or overfitting is present. This is particularly important for smaller datasets.
  * Exploring the implications of applying Label Encoding to numerical features, and consider if standard numerical processing would be more appropriate.
  * Implementing cross-validation for more robust model evaluation.
  * Adding explainability (e.g., SHAP or LIME) to understand which physical measurements are most discriminatory between the penguin species.
