
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

| Task                                         | Model(s) Used                                                                                                    |
| -------------------------------------------- | -------------------------------------------------------------------------------                                  |
| **Disease Risk Prediction (Classification)** | Logistic Regression, Support Vector Machine (SVM), **Random Forest Classifier**, Decision Tree                   |
| **Expense Prediction (Regression)**          | **Linear Regression**, Random Forest Regressor, Ridge Regression, Lasso Regression,ElasticNet Regression,        |
| **Patient Risk Grouping (Clustering)**       | K-Means Clustering                                                                                               |

---

# 🔍 Model Performance Analysis

### 1️⃣ **Classification Models — Disease Risk Prediction**

| Model                        | Performance Summary                                                                                             | Verdict                            |
| ---------------------------- | --------------------------------------------------------------------------------------------------------------- | ---------------------------------- |
| **Logistic Regression**      | Performs adequately as a baseline but limited in capturing non-linear relationships.                            | **Baseline Model**                 |
| **Decision Tree Classifier** | Offers interpretability with moderate performance; prone to overfitting.                                        | **Acceptable but not recommended** |
| **Support Vector Machine**   | Shows consistently strong accuracy and F1-score; handles complex decision boundaries effectively.               | **Recommended Model**              |
| **Random Forest Classifier** | Provides the highest accuracy and generalization; robust to noise and overfitting due to ensemble architecture. | ⭐ **Best Overall Model**           |


---

### 2️⃣ **Regression Models — Medical Expense Prediction****

| Model                       | Performance Summary                                                                   | Verdict                          |
| --------------------------- | ------------------------------------------------------------------------------------- | -------------------------------- |
| **Linear Regression**       | Establishes a baseline with moderate R²; limited with non-linear patterns.            | **Baseline Model**               |
| **Ridge Regression**        | Stabilizes coefficients via L2 regularization; marginal improvement over baseline.    | **Reliable Regularized Model**   |
| **Lasso Regression**        | Similar performance to Ridge; performs feature selection effectively.                 | **Useful for Feature Reduction** |
| **ElasticNet Regression**   | Combines L1 + L2 regularization; best-performing linear model in this task.           | **Strong Linear Model**          |
| **Random Forest Regressor** | Captures complex, non-linear patterns well and achieves one of the highest R² scores. | ⭐ **Best Overall Model**         |



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
| **Healthcare Expense Prediction** | **Random Forest Regressor**  | Best R² and lowest MSE (most reliable estimation)      |
| **Patient Segmentation**          | **K-Means Clustering**       | Clear and meaningful grouping of patient risk profiles |

---

## 🧰 Tech Stack

* Python (Pandas, NumPy, Scikit-Learn)
* Matplotlib / Seaborn (Visualization)
* Google Colab

