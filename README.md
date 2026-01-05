# credit-card-fraud-detection
Machine learning-based credit card fraud detection using Random Forest on imbalanced dataset

## Key Results 
  - **Random Forest** detected **73 out of 98 fraudulent transaction (74.5% recall)
  - Achieved **96% precision**  with only **3 false positives**
  - Logistic Regression baseline detected only **2** fraud cases

## Visuals

## Feature Importances

![Feature Importance]
<img width="790" height="631" alt="Screenshot 2026-01-05 at 3 19 38 pm" src="https://github.com/user-attachments/assets/810a5866-d4d3-4524-a991-dcc301fbe40f" />

## Model Comparison
![Model Confusion Table]
<img width="438" height="215" alt="Screenshot 2026-01-05 at 3 20 35 pm" src="https://github.com/user-attachments/assets/ec53076b-3290-474a-a19c-4c95d5c3f043" />


## Correlation Heatmap
![Correlation Heatmap] 
<img width="761" height="696" alt="Screenshot 2026-01-05 at 12 08 48 pm" src="https://github.com/user-attachments/assets/ba81d757-2108-4f7d-85eb-428f04fee7e0" />


## Approach
  - Handled severe class imbalance using 'class_weight='balanced'' in the scikit-learn
  - Models compared: Logistic Regression (baseline) vs Random Forest
  - Evalution focused on precision, recall, and false positives (not accuracy)
  - Feature importance from Random Forest highlighted V14 and V10 as top predictors

## Exploratory Data Analysis & Statistical Validation in R

Visualized key patterns and confirmed statistical significance in R:

### Class Imbalance
![Class Distribution]
<img width="3000" height="1800" alt="fraud_class_distribution" src="https://github.com/user-attachments/assets/5eb74a7a-fe69-457f-b819-f70afff9d867" />


### Transaction Amount by Class
![Amount Box Plot]
<img width="3000" height="1800" alt="fraud_amount_distribution" src="https://github.com/user-attachments/assets/51d476d6-4a17-4f9f-a1bc-591b1f72e1bc" />


![Amount Histogram]
<img width="3000" height="1800" alt="fraud_amount_boxplot" src="https://github.com/user-attachments/assets/8263a646-b07b-479f-80aa-9c34f0885cda" />



## Tech Stack
  - **Python**: scikit-learn, pandas, seaborn, matplotlib
  - **R**: Statistical testing and additional visualizations

## How to Run 
```bash
pip install -r requirement.txt
jupyter notebook fraud_detection.ipynb
  
