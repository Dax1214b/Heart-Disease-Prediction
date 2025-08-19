# Heart Disease Prediction (Machine Learning)

This project uses <b>Machine Learning algorithms</b> to predict the likelihood of heart failure based on clinical data.<br>
The dataset includes patient information such as age, blood pressure, diabetes, smoking status, and laboratory measurements.

---

## 📂 Dataset
The dataset contains <b>299 patient records</b> with the following features:<br>

- <b>age</b> — Age of the patient  
- <b>anaemia</b> — Whether the patient has anemia (0 = No, 1 = Yes)  
- <b>creatinine_phosphokinase</b> — Level of CPK enzyme in blood  
- <b>diabetes</b> — Diabetes status (0 = No, 1 = Yes)  
- <b>ejection_fraction</b> — Percentage of blood leaving the heart each time it contracts  
- <b>high_blood_pressure</b> — Hypertension status (0 = No, 1 = Yes)  
- <b>platelets</b> — Platelet count in the blood  
- <b>serum_creatinine</b> — Level of serum creatinine in blood  
- <b>serum_sodium</b> — Level of serum sodium in blood  
- <b>sex</b> — Gender (0 = Female, 1 = Male)  
- <b>smoking</b> — Smoking status (0 = No, 1 = Yes)  
- <b>time</b> — Follow-up period (days)  
- <b>DEATH_EVENT</b> — <i>Target variable</i> (0 = Alive, 1 = Death)  

---

## ⚙️ Steps in the Project
1. <b>Data Preprocessing</b><br>
   - Checked for missing values  
   - Split dataset into features (<i>X</i>) and target (<i>y</i>)  
   - Applied train-test split with stratification  

2. <b>Feature Scaling</b><br>
   - Used <code>StandardScaler</code> for Logistic Regression  
   - Random Forest does not require scaling  

3. <b>Model Training</b><br>
   - Logistic Regression (baseline linear model)  
   - Random Forest Classifier (ensemble model with 200 trees)  

4. <b>Model Evaluation</b><br>
   - Accuracy score on test data  
   - Logistic Regression and Random Forest compared  
   - Random Forest achieved ~<b>81%</b> accuracy  

5. <b>Making Predictions</b><br>
   - Scaled new patient input for Logistic Regression  
   - Passed raw feature DataFrame for Random Forest  

---

## 📊 Results
- <b>Logistic Regression</b>: Accuracy ≈ (depends on run)  
- <b>Random Forest</b>: Accuracy ≈ <b>81%</b>  

<i>Note:</i> Models can sometimes disagree on borderline patient cases.<br>

---



