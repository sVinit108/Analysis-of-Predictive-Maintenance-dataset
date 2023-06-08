# Analysis-of-Predictive-Maintenance-dataset

Apart from building a prediction ML model, a detailed data analysis is done to get insightful information
from the dataset. All stages of ML life‑cycle (Feature engineering,
Feature selection, Model creation, hyparameter tuning & Cross Validation) is
performed on the dataset. <br>

BACKGROUND:- A company has a fleet of devices transmitting daily
sensor readings. They would like to create a predictive maintenance
solution to proactively identify when maintenance should be
performed. This approach promises cost savings over routine or time based preventive maintenance, because tasks are performed only when
warranted. <br>

GOAL:- You are tasked with building a predictive model using machine
learning to predict the probability of a device failure. When building
this model, be sure to minimize false positives and false negatives. The
column you are trying to Predict is called failure with binary value 0 for
non-failure and 1 for failure. 

#   Steps Followed
1. Feature Engineering
    - EDA (Numerical-Categorical variables separation & null-value containig feature detection, Feature's value distribution analysis, Missing value analysis, Outlier analysis, Feature relation study)
    - Missing Values (None present)
    - Outliers handling (By replacing with 15 & 85 quartile value)
    - Encoding (Not required since all numerical varibles are present)
    - Checeking if case of Anamoly Detection (This was done by checking whether the values of metrics are outliers in case of failed device)
    - Scaling (Different Transformation techniques were applied & the best one was picked. Q-Q plots were also plotted.)
    - Imbalaced data checking
    
2. Feature Selection
    - Dropping feauteres with low variance
    
3. Model Creation
    - Random forest
    - Gradient Boosting Algorithm

4. Cross Validation
    - Using repeated train-test split
    
5. Hyperparameter tuning
    - RandomizedSearchCV
