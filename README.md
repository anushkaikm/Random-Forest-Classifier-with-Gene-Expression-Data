# Random Forest Classifier with Gene Expression Data

## Overview
This project explores the use of a **Random Forest Classifier** for analyzing gene expression data to classify samples into distinct categories. Inspired by the paper *"Cell Type Discovery Using Single-Cell Transcriptomics: Implications for Ontological Representation"*, this experiment focuses on:
- **Feature Ranking:** Identifying the most important features (genes) using Gini and Permutation Importance.
- **Model Evaluation:** Employing metrics like confusion matrices, ROC curves, and classification reports to ensure robust performance.

## Key Features
- Utilizes **Scikit-learn's Random Forest Classifier** for feature importance analysis and classification.
- Implements **GridSearchCV** for hyperparameter tuning.
- Employs both **Cross-Validation (CV)** and **Out-of-Bag (OOB)** error estimation for unbiased accuracy assessment.
- Analyzes the **biological relevance** of top-ranked genes to validate the model's findings.

## Dataset
- **Source:** Inspired by the paper mentioned above.
- **Structure:** Contains 871 samples and 608 features (gene expression data), split into two classes.
- **Class Distribution:** Class 0 (572 samples), Class 1 (299 samples).

## Methodology
1. **Data Preprocessing:** Ensured no missing values and normalized data.
2. **Hyperparameter Tuning:** Optimized `n_estimators`, `max_features`, and `max_depth` using GridSearchCV.
3. **Evaluation Metrics:**
   - Confusion Matrix
   - ROC Curve and AUC
   - Classification Report (Precision, Recall, F1-Score)
4. **Feature Ranking:** Compared Gini Importance and Permutation Importance to identify top-performing features.

## Results
- **Model Accuracy:** Achieved 100% accuracy on the test set.
- **OOB Score:** 0.9939, reflecting a high level of confidence in model generalization.
- **Feature Insights:** Top features, such as TESPA1, SLC17A7, and LINC00507, align with known biological functions.

## Tools and Resources
- **Language & Frameworks:**
  - Python (Jupyter Notebook)
  - Scikit-learn
- **References:**
  - [Scikit-learn Documentation](https://scikit-learn.org)
  - [Feature Importance in Random Forest](https://mljar.com/blog/feature-importance-in-random-forest/)
- **Visualization:**
  - Confusion Matrix and ROC Curve plots
- **Adviser:** ChatGPT, for drafting explanations and optimizing code.

---
## Acknowledgments
Special thanks to:
- Professor Dragutin Petkovic for guidance.
- Zoe Long, Rongxian Tong, and Rosaclaire Baisinger for their support.
- ChatGPT for assistance in refining code and documentation.

