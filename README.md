# Analysis of Predictive Maintenance Dataset

This project focuses on building a **predictive maintenance solution** using machine learning, supported by **in-depth exploratory data analysis (EDA)** and a complete ML lifecycle pipeline.

Beyond model building, the emphasis is on **extracting meaningful insights from sensor data** and making principled modeling decisions at each stage.

---

## Background

A company operates a fleet of devices that transmit **daily sensor readings**.  
The objective is to develop a predictive maintenance system that can **proactively identify potential device failures**, enabling maintenance to be performed **only when required**.

This approach aims to reduce costs compared to routine or time-based preventive maintenance strategies.

---

## Goal

To build a machine learning model that predicts the **probability of device failure**, where:

- `0` → Non-failure  
- `1` → Failure  

Special care is taken to **minimize both false positives and false negatives**, as both have significant operational impact.

---

## Methodology

The project follows all major stages of the **machine learning lifecycle**.

### 1. Feature Engineering

- **Exploratory Data Analysis (EDA):**
  - Numerical vs categorical variable analysis  
  - Missing value assessment  
  - Feature distribution analysis  
  - Outlier detection  
  - Feature relationship study  

- **Missing Values:**  
  - No missing values present in the dataset  

- **Outlier Handling:**  
  - Outliers treated using **15th and 85th percentile capping**  

- **Encoding:**  
  - Not required (all features are numerical)  

- **Anomaly Detection Check:**  
  - Investigated whether failed devices exhibit anomalous sensor readings  

- **Scaling:**  
  - Multiple transformation techniques evaluated  
  - Best transformation selected using **Q–Q plots**  

- **Class Imbalance Analysis:**  
  - Checked and accounted for imbalance in failure labels  

---

### 2. Feature Selection

- Removed features with **low variance** to reduce noise and redundancy  

---

### 3. Model Development

The following models were trained and evaluated:

- Random Forest  
- Gradient Boosting  

---

### 4. Cross Validation

- Performance evaluated using **repeated train–test splits** to ensure robustness  

---

### 5. Hyperparameter Tuning

- Hyperparameters optimized using **RandomizedSearchCV**  

---

## Results & Insights

- Combined EDA and modeling provided strong intuition about **sensor behavior prior to failure**
- Ensemble models performed better than simpler baselines
- Proper preprocessing significantly improved model stability and generalization

---

## Project Context

This project was developed as part of an **internal hackathon**.  
I received **special appreciation from the instructor** for:
- Clarity of explanation  
- Depth of subject understanding  
- Effectiveness in presenting data-driven insights  

---

## Tech Stack

- Python  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib / Seaborn  
- Jupyter Notebook  

---

## Author

**Vinit Sharma**  
M.Tech (AI & Data Science), VJTI Mumbai  
GitHub: https://github.com/sVinit108
