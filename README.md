# Classification-Metabolic-Syndrome-Prediction
## Analyzing Key Risk Factors and Demographics to Predict the Presence of Metabolic Syndrome in Patients

**Author**: Brooke Eagan

### Business problem:
To provide the best care, different health and demographic factors are used to create a machine learning model to predict whether a patient has developed metabolic syndrome.



### Data:
Metabolic Syndrome Dataset https://data.world/informatics-edu/metabolic-syndrome-prediction

This dataset contains 2401 row and 15 columns. The rows represent 2401 patients and the columns represent 14 features and 1 target.
### Data Dictionary
<p align = "center"> 
  <img src = "Metabolic Syndrome Data Dictionary.png"> 
</p>

## Methods
- To prepare this data, the data was cleaned, and the following processes were performed:
  - Column names and datatypes were inspected and corrected 
  - Values and value datatypes were inspected and corrected
  - The dataset was split into training and test sets for classification models

## Exploratoy Data Analysis
- A boxplot for age, ration of albumin to creatine in urine, blood glucose, HDL, and triglycerides were visualized.
- A histogram for income, waist circumference, and uric acid were visualized.
- A count plot for albunin in urine, sex, race, marital status were visualized.
- Outliers were calculated.


#### How Many Patients Have Metablolic Syndrome?
<p align = "center"> 
  <img src = "Metabolic Syndrome Count Plot.png">
</p>

-Most patients do not have metabolic syndrome.

## Explanatory 

#### What Health Factors Indicate Metabolic Syndrome Diagnosis?
<p align = "center"> 
  <img src = "https://raw.githubusercontent.com/Beagan19/Classification-Metabolic-Syndrome-Prediction/main/Presence of Metabolic Syndrome Based on Risk Factors.png">
</p>

- The higher the numbers are for blood glucose, bmi, and triglycerides for both males and females, the more likely a patient developed metabolic syndrome.
- The higher the numbers for HDL for both males and females, the more likely a patient does not develop metabolic syndrome.
### Do Demographics Play a Part in Developing Metabolic Syndrome?
<p align = "center"> 
  <img src = "Presence of Metabolic Syndrome Based on Demographics.png">
</p>

- An older age could have an impact on whether a patient developed metabolic syndrome for both males and femaales.

- Income is approximately equivalent for males with and without metabolic syndrome. However, a higher income for females could decrease the possibility of developing metabolic syndrome.
## Models Evaluated & Results
- Logistic Regression:
  - accuracy: 0.82

- f1-score:
  - MetSyn     0.74
  - No MetSyn  0.87
  
- precision:
  - MetSyn     0.76
  - No MetSyn  0.86

- recall:
  - MetSyn     0.72
  - No MetSyn  0.88

- Random Forest Classifier:
  - accuracy: 0.81

  - f1-score:
    - MetSyn     0.73
    - No MetSyn  0.85
  
  - precision:
    - MetSyn     0.71
    - No MetSyn  0.86

  - recall:
    - MetSyn     0.74
    - No MetSyn  0.85

The Final Model Chosen was a Logistic Regression Model with the inverse of regulation strength ('c') was tuned to .06. The pca n_components was tuned to 11. 'Most frequent' was the strategy used to impute missing numeric values. 

## Recommended Model: Logistic Regression
- It has the highest accuracy score and f1-score. It is important to minimize the number of false positives and false negatives when dianosing a disease so both type 1 and type 2 errors need to be examined.

**Tuned Logistic Regression Model Test Scores**

- accuracy:
  - 0.82

- f1-score:
  - MetSyn     0.74
  - No MetSyn  0.87
  
- precision:
  - MetSyn     0.76
  - No MetSyn  0.86

- recall:
  - MetSyn     0.72
  - No MetSyn  0.88


## Limitations & Next Steps

With hypertuning parameters, I was not able to exceed 82% accuracy. The first step would be to add columns to the data using feature engineering. Then tune and run the models again to try to obtain better prediction results.


### For further information


For any additional questions, please contact:

Brooke Eagan
brooke.eagan4@gmail.com
