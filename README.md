
# 🏥 Smart Healthcare Expense & Disease Prediction System (Machine Learning Project)

This project is a **Machine Learning-based Healthcare Decision Support System** that analyzes patient data to:

1. **Predict Health Risk** (Classification)
2. **Estimate Healthcare / Medical Insurance Expenses** (Regression)
3. **Group Patients into Risk Segments** (Clustering)
4. **Provide Lifestyle & Health Improvement Suggestions**

The system is **fully data-driven** and requires only patient health parameters as input.
**No IoT / Sensors / Hardware involvement.**

---

## 🧠 Core Functionalities

| Module                        | Purpose                                                       | Output                                              |
| ----------------------------- | ------------------------------------------------------------- | --------------------------------------------------- |
| **Health Prediction**         | Classifies risk levels based on patient health indicators.    | Risk Category: Low / Medium / High                  |
| **Expense Prediction**        | Predicts medical insurance cost or expected medical spending. | Estimated Expense (₹ / $)                           |
| **Patient Segmentation**      | Groups patients with similar risk characteristics.            | Cluster Group (Healthy / Moderate Risk / High Risk) |
| **Lifestyle Recommendations** | Suggests improvements to reduce disease risk.                 | Diet, Exercise & Habit Modifications                |

---

## 🔄 Project Workflow

1. Data Cleaning & Preprocessing  
2. Exploratory Data Analysis (EDA)  
3. Feature Encoding & Scaling  
4. Model Training (Classification, Regression, Clustering)  
5. Model Evaluation & Comparison  
6. Final Model Selection  

---

## 🩺 Input Patient Features

* Age
* Gender
* BMI
* Blood Pressure
* Sugar / Cholesterol Levels
* Physical Activity Level
* Smoking / Alcohol Usage
* Family Medical History

---
## 📁 Dataset Overview

- **Dataset Shape:** (1338, 7)
- **Records:** 1338 patient entries
- **Features:**
  - Age
  - Sex
  - BMI
  - Number of Children
  - Smoking Status
  - Region
- **Target Variable:**
  - Charges (Medical Insurance Cost)

### 🎯 Purpose
The dataset is used to analyze patient demographic and lifestyle factors to:
- Estimate medical insurance expenses using regression models
- Assess health risk patterns associated with factors such as smoking, BMI, and age
- Support data-driven healthcare cost prediction and patient risk segmentation


## 📊 Machine Learning Models Used

| Task                                         | Model(s) Used                                                                                                    |
| -------------------------------------------- | -------------------------------------------------------------------------------                                  |
| **Health Risk Prediction (Classification)**  | Logistic Regression, Support Vector Machine (SVM), **Random Forest Classifier**, Decision Tree                   |
| **Expense Prediction (Regression)**          | **Linear Regression**, Random Forest Regressor, Ridge Regression, Lasso Regression,ElasticNet Regression,        |
| **Patient Risk Grouping (Clustering)**       | K-Means Clustering                                                                                               |

---

# 🔍 Model Performance Analysis

### 1️⃣ **Classification Models — Health Risk Prediction**

| Model                        | Performance Summary                                                                                             | Verdict                            |
| ---------------------------- | --------------------------------------------------------------------------------------------------------------- | ---------------------------------- |
| **Logistic Regression**      | Performs adequately as a baseline but limited in capturing non-linear relationships.                            | **Baseline Model**                 |
| **Decision Tree Classifier** | Offers interpretability with moderate performance; prone to overfitting.                                        | **Acceptable but not recommended** |
| **Support Vector Machine**   | Shows consistently strong accuracy and F1-score; handles complex decision boundaries effectively.               | **Recommended Model**              |
| **Random Forest Classifier** | Provides the highest accuracy and generalization; robust to noise and overfitting due to ensemble architecture. | ⭐ **Best Overall Model**           |

**Random Forest Classifier (Best Model):**
- Accuracy: ~89%
- Precision: ~90%
- Shows strong ability to correctly identify high-risk cases with minimal false positives

---

### 2️⃣ **Regression Models — Medical Expense Prediction**

| Model                       | Performance Summary                                                                   | Verdict                          |
| --------------------------- | ------------------------------------------------------------------------------------- | -------------------------------- |
| **Linear Regression**       | Establishes a baseline with moderate R²; limited with non-linear patterns.            | **Baseline Model**               |
| **Ridge Regression**        | Stabilizes coefficients via L2 regularization; marginal improvement over baseline.    | **Reliable Regularized Model**   |
| **Lasso Regression**        | Similar performance to Ridge; performs feature selection effectively.                 | **Useful for Feature Reduction** |
| **ElasticNet Regression**   | Combines L1 + L2 regularization; best-performing linear model in this task.           | **Strong Linear Model**          |
| **Random Forest Regressor** | Captures complex, non-linear patterns well and achieves one of the highest R² scores. | ⭐ **Best Overall Model**         |


**Random Forest Regressor (Best Model):**
- R² Score: 0.5607
- Mean Squared Error (MSE): 2740.44



---

### 3️⃣ **Clustering — Patient Grouping & Risk Segmentation**

| Model                  | Output Interpretation                                                                          |
| ---------------------- | ---------------------------------------------------------------------------------------------- |
| **K-Means Clustering** | Successfully formed **3 natural patient clusters**: Low Risk, Moderate Risk, High Risk groups. |

Clustering helps in:

* Identifying which group a patient belongs to
* Designing preventive healthcare plans
* Targeted awareness or intervention programs

---

## ✅ **Final Combined Conclusion**

| Task                              | Best Performing Model        | Reason                                                 |
| --------------------------------- | ---------------------------- | ------------------------------------------------------ |
| **Health Risk Prediction**        | **Random Forest Classifier** | Accuracy: ~89% (better then rest), Precision: 90%      |
| **Healthcare Expense Prediction** | **Random Forest Regressor**  | Better R² (0.5607) and lowest MSE (2740.44)            |
| **Patient Segmentation**          | **K-Means Clustering**       | Clear and meaningful grouping of patient risk profiles |

---

## ⚠️ Limitations

- Dataset size is relatively small (1338 records), which may limit generalization.
- Health risk is inferred indirectly from demographic and lifestyle factors, not clinical diagnoses.
- Model performance may vary on unseen real-world healthcare data due to limited dataset diversity.

---

## 🔮 Future Improvements

- Integrate larger and more diverse healthcare datasets.
- Include explainability tools (SHAP) to interpret model predictions.

---

## 🧰 Tech Stack

### Programming Language
- Python

### Data Analysis & Preprocessing
- Pandas
- NumPy

### Machine Learning & Modeling
- scikit-learn
  - Logistic Regression
  - Support Vector Machine (SVM)
  - Decision Tree Classifier
  - Random Forest Classifier & Regressor
  - Linear Regression
  - Ridge Regression
  - Lasso Regression
  - ElasticNet Regression
  - K-Means Clustering

### Data Visualization
- Matplotlib
- Seaborn

### Model Evaluation
- Accuracy Score
- Precision
- R² Score
- Mean Squared Error (MSE)

### Development Environment
- Google Colab
- Jupyter Notebook

### Version Control
- Git
- GitHub


---

## 🚀 How to Run the Project

1. Clone the repository  
2. Install dependencies  
   `pip install -r requirements.txt`  
3. Open the Jupyter notebook and run all cells sequentially



