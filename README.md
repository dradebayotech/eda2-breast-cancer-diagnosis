# 🩺 EDA PROJECT 2:
#  Unveiling Insights for Breast Cancer Diagnosis: An Exploratory Data Analysis

## 📌 Project Overview
This project represents a focused effort to conduct an in-depth Exploratory Data Analysis (EDA) on a vital Breast Cancer Diagnosis dataset. My goal is to move beyond surface-level statistics and truly understand the intricate characteristics that distinguish benign (non-cancerous) from malignant (cancerous) tumors, utilizing features derived from digitized images of fine needle aspirates (FNA). Through meticulous data inspection, cleaning, and compelling visualizations, I aim to uncover critical patterns and relationships. These insights are not merely academic; they are the foundational steps in building a robust predictive model, a tool that holds the potential to contribute to more accurate and timely breast cancer diagnoses. This project is a personal commitment to leveraging data science for impactful contributions in healthcare.

This project is part of my **data science portfolio**

---

## 🧰 Tools & Libraries
- **Python** (Jupyter Notebook)  
- **pandas** and **numpy** for data wrangling  
- **matplotlib** and **seaborn** for visualization
- **GitHub** for portfolio showcase

---

## ❓ Key Exploratory Questions Addressed

This analysis was guided by the following nine scientific/research questions, aimed at uncovering data patterns and relationships relevant to breast cancer diagnosis:

1. **What is the Diagnosis Distribution of the Tumor Types (M = Malignant, B = Benign)?**  
2. **What can you deduce from the descriptive statistics (mean, standard deviation, and skewness) for the 'mean' features in the breast cancer dataset?**  
3. **What can you deduce from the descriptive statistics (mean, standard deviation, and skewness) for the 'worst' features in the breast cancer dataset?**  
4. **How do the distributions of the top 6 mean features differ between benign and malignant tumors?**  
5. **How do the distributions of various breast cancer features (such as radius, texture, perimeter, etc.) differ between benign and malignant tumors?**  
6. **How are the various features correlated with each other and with the diagnosis?**  
7. **What are the shapes and ranges of the distributions for key features when separated by diagnosis?**  
8. **How do pairs of features relate to each other, and does the relationship differ based on the diagnosis?**  
9. **How do the correlations between pairs of features differ between malignant and benign tumors?**

Each question was explored using descriptive statistics, visualizations, and correlation analyses to uncover clinically meaningful insights.

---

## 🔍 Key Analysis Steps
1. **Data Inspection**
   - Dataset contains **569 samples** and **33 features** (including ID and diagnosis).
   - One column (`Unnamed: 32`) contained no values and was dropped.
   - Identified datatype mismatches across numeric and categorical fields.

2. **Data Cleaning**
   - Removed redundant/unnecessary columns.  
   - Checked for and handled missing/empty values.  

3. **Exploratory Visualizations**
   - Class distribution between benign and malignant tumors.
   - Correlation heatmap of all features.  
   - Boxplots of critical features across diagnosis classes.  
   - Pairplots of selected features to study separability.  
   - And so on.

---

## 📊 Insights
- **Class Distribution:** The dataset is slightly imbalanced but still workable for modeling.  
- **Correlated Features:** Strong relationships exist among *radius, perimeter, and area* features, which may influence feature selection.  
- **Scaling Needs:** Features have widely varying ranges, highlighting the need for scaling before predictive modeling.  
- **Feature Separability:** Certain features (e.g., `concave points_worst`, `area_worst`) strongly separate benign vs malignant tumors.  

---

## 📸 Sample Visuals from the Notebook  

| Class Distribution | Correlation Heatmap |
|--------------------|---------------------|
| ![Class Distribution](Images/class_distribution.png) | ![Heatmap](Images/feature_correlation_heatmap.png) |

| Boxplot of Features | Pairplot of Key Features |
|----------------------|--------------------------|
| ![Boxplot](Images/boxplot_selected_features.png) | ![Pairplot](Images/pairplot_key_features.png) |


---

## 📁 Files in This Repository
- `EDA_Project2.ipynb`: Jupyter notebook with full exploratory analysis  
- `Images/`: Folder containing exported plots used in README  
- `Data/`: Folder with sample CSVs (dataset uploaded here)  

---

## 📂 Dataset Access
You can access or download it here:  
👉 [Breast Cancer Wisconsin (Diagnostic) Dataset on Kaggle](https://www.kaggle.com/datasets/wasiqaliyasir/breast-cancer-dataset)  

---

## 📊 Key Findings and Significant Implications for the development of a Predictive Model

**Based on the Exploratory Data Analysis of the Breast Cancer Diagnosis dataset, some of the key findings and implications for building a predictive model are as follows:**

- The dataset exhibits class imbalance, with significantly more benign cases than malignant ones, which will require consideration during model training (e.g., using techniques like stratification, resampling, or adjusting class weights).
- Many features show distinct distributions and significantly different mean and median values between benign and malignant tumors, particularly features related to the size and irregularity of cell nuclei (radius, perimeter, area, concave points, and their 'worst' counterparts). These features are likely to be strong predictors of diagnosis.
- High correlations exist among many features, especially within the 'mean' and 'worst' groups, suggesting potential multicollinearity. This might necessitate feature selection or dimensionality reduction techniques to improve model stability and interpretability.
- The differential correlation analysis revealed that the relationships between some feature pairs change significantly between benign and malignant tumors, providing further discriminatory information that a model could leverage.
- The presence of outliers, especially in malignant cases for certain features, indicates data variability and might require robust preprocessing steps or models less sensitive to extreme values.
- The clear separation observed in pairwise plots for several feature combinations reinforces their potential as powerful discriminators for classifying tumor type.

**Overall, the EDA suggests that a predictive model should focus on features related to cell morphology and nuclear characteristics, while also addressing class imbalance and potential multicollinearity to achieve accurate and reliable breast cancer diagnosis prediction.**

---

## 🚀 Next Steps
- Build baseline ML classifiers (Logistic Regression, Random Forest, XGBoost).  

---
## ✍️ Author
**Adebayo Fashina**  
📍 Toronto, Canada | [LinkedIn](https://www.linkedin.com/in/your-link-here)  

