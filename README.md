
# 🏥 Smart Healthcare Expense & Disease Prediction System (Machine Learning Project)

This project is a **Machine Learning-based Healthcare Decision Support System** that analyzes patient data to:

1. **Predict Disease Risk** (Classification)
2. **Estimate Healthcare / Medical Insurance Expenses** (Regression)
3. **Group Patients into Risk Segments** (Clustering)
4. **Provide Lifestyle & Health Improvement Suggestions**

The system is **fully data-driven** and requires only patient health parameters as input.
**No IoT / Sensors / Hardware involvement.**

---

## 🧠 Core Functionalities

| Module                        | Purpose                                                       | Output                                              |
| ----------------------------- | ------------------------------------------------------------- | --------------------------------------------------- |
| **Disease Prediction**        | Classifies risk levels based on patient health indicators.    | Risk Category: Low / Medium / High                  |
| **Expense Prediction**        | Predicts medical insurance cost or expected medical spending. | Estimated Expense (₹ / $)                           |
| **Patient Segmentation**      | Groups patients with similar risk characteristics.            | Cluster Group (Healthy / Moderate Risk / High Risk) |
| **Lifestyle Recommendations** | Suggests improvements to reduce disease risk.                 | Diet, Exercise & Habit Modifications                |

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

## 📊 Machine Learning Models Used

| Task                                         | Model(s) Used                                                                   |
| -------------------------------------------- | ------------------------------------------------------------------------------- |
| **Disease Risk Prediction (Classification)** | Logistic Regression, Support Vector Machine (SVM), **Random Forest Classifier** |
| **Expense Prediction (Regression)**          | **Linear Regression**, Decision Tree Regressor, Random Forest Regressor         |
| **Patient Risk Grouping (Clustering)**       | K-Means Clustering                                                              |

---

# 🔍 Model Performance Analysis

### 1️⃣ **Regression Models — Medical Expense Prediction**

| Model                   | Performance Summary                                                         | Conclusion                              |
| ----------------------- | --------------------------------------------------------------------------- | --------------------------------------- |
| **Linear Regression**   | Achieved **highest R² score** and **lowest MSE**. Stable and interpretable. | ✅ **Best Model for Expense Prediction** |
| Decision Tree Regressor | Moderate performance but **high overfitting**.                              | Not recommended for final prediction.   |
| Random Forest Regressor | Good accuracy but slightly less stable than Linear Regression.              | Suitable but not optimal.               |

> **Final Choice for Regression:**
> ➡️ **Linear Regression** — Best accuracy & reliability in predicting healthcare expenses.

---

### 2️⃣ **Classification Models — Disease Risk Prediction**

| Model                        | Performance Summary                                                       | Conclusion                                       |
| ---------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------ |
| Logistic Regression          | Works as a baseline model but limited in handling complex patterns.       | Basic, less accurate.                            |
| Support Vector Machine (SVM) | Higher accuracy but **slower computation**.                               | Good but less efficient.                         |
| **Random Forest Classifier** | **Highest accuracy**, best precision-recall, **low overfitting**, stable. | ✅ **Best Model for Disease Risk Classification** |

> **Final Choice for Classification:**
> ➡️ **Random Forest Classifier** — Most stable and accurate for predicting disease risk levels.

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
| **Disease Risk Prediction**       | **Random Forest Classifier** | Highest predictive stability & classification accuracy |
| **Healthcare Expense Prediction** | **Linear Regression**        | Best R² and lowest MSE (most reliable estimation)      |
| **Patient Segmentation**          | **K-Means Clustering**       | Clear and meaningful grouping of patient risk profiles |

---

## 🧰 Tech Stack

* Python (Pandas, NumPy, Scikit-Learn)
* Matplotlib / Seaborn (Visualization)
* Jupyter Notebook / Google Colab

