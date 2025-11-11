



# 🎓 Student Performance Prediction using Machine Learning

This project analyzes and predicts students’ academic performance using the **UCI Student Performance Dataset**.  
It applies regression and classification models to understand factors influencing grades and predict final exam results.

---

## 📂 Project Overview

The dataset includes information about students’ demographics, family background, study habits, and academic scores.  
We perform data preprocessing, visualization, and train multiple machine learning models to predict:

- **Final grade (G3)** using **Linear Regression**
- **Pass/Fail classification** using **Logistic Regression** and **Decision Tree Classifier**

---

## 🧠 Objectives

- Explore and clean the dataset  
- Visualize key relationships between features and performance  
- Build regression and classification models  
- Evaluate and compare model performance  
- Identify key predictors of student success  

---

## 📊 Dataset Information

- **Source:** [UCI Machine Learning Repository - Student Performance Dataset](https://archive.ics.uci.edu/ml/datasets/Student+Performance)  
- **Attributes:** 33 features (demographic, social, and academic factors)  
- **Target Variables:**
  - `G3`: Final grade (for regression)
  - `pass_fail`: 1 = Pass (G3 ≥ 10), 0 = Fail (G3 < 10)

---

## ⚙️ Technologies Used

- **Python 3**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Scikit-learn**
- **ucimlrepo**

---

## 🚀 Workflow Summary

1. **Data Loading**
   - Loaded the dataset using `ucimlrepo` (fallback: UCI URL).

2. **Data Preprocessing**
   - Encoded categorical variables with `LabelEncoder`
   - Created a new binary column: `pass_fail`
   - Scaled features with `StandardScaler`

3. **Exploratory Data Analysis (EDA)**
   - Correlation heatmap
   - Study time vs final grade scatterplot

4. **Model Training**
   - **Linear Regression** → Predict final marks (G3)
   - **Logistic Regression** → Classify Pass/Fail
   - **Decision Tree Classifier** → Classify Pass/Fail

5. **Evaluation**
   - Metrics: Accuracy, Precision, Recall, MSE, R² Score
   - Confusion Matrix Visualization

---

## 📈 Results

| Model | Accuracy | Precision | Recall |
|--------|-----------|------------|--------|
| Logistic Regression | 0.92 | 0.96 | 0.96 |
| Decision Tree | 0.91 | 0.95 | 0.95 |

### 🧩 Key Findings:
- Linear Regression achieved **R² = 0.86**, indicating strong predictive power for final grades.  
- Logistic Regression and Decision Tree both performed well in classification tasks.  
- **Study time**, **previous grades (G1, G2)**, and **absences** were strong predictors of student outcomes.  

---

## 📉 Visualizations

- 📊 **Feature Correlation Heatmap**  
- 🧮 **Study Time vs Final Grade Scatterplot**  
- 🔍 **Decision Tree Confusion Matrix**

---

## ✅ Conclusion

- Linear Regression predicted students’ marks with high accuracy.  
- Logistic Regression and Decision Tree effectively classified students as Pass/Fail.  
- Decision Tree performed slightly better in precision and recall.  
- Study habits and prior academic performance strongly influence success.

---

## 📘 How to Run

```bash
# Clone the repository
git clone https://github.com/your-username/student-performance-ml.git

# Navigate to the project folder
cd student-performance-ml

# Install dependencies
pip install -r requirements.txt

# Run the Jupyter notebook
jupyter notebook student_performance.ipynb
