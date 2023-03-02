# Classification-Metabolic-Syndrome-Prediction
## Analyzing Key Risk Factors and Demographics to Predict the Presence of Metabolic Syndrome 

**Author**: Brooke Eagan

### Business problem:

Here is where you state the business problem you were trying to solve


### Data:
Metabolic  Syndrome.csv
This dataset contains 2401 row and 15 columns. The rows represent 2401 patients and the columns represent 14 features and 1 target.
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
  <img src = "https://raw.githubusercontent.com/Beagan19/Classification-Metabolic-Syndrome-Prediction/main/Metabolic Syndrome Count Plot.png">
</p>

-Most patients do not have metabolic syndrome.

#### What Factors Indicate Metabolic Syndrome Diagnosis?
<p align = "center"> 
  <img src = "https://raw.githubusercontent.com/Beagan19/Classification-Metabolic-Syndrome-Prediction/main/Presence of Metabolic Syndrome Based on Risk Factors.png">
</p>

- The higher the numbers are for blood glucose, bmi, and triglycerides for both males and females, the more likely a patient developed metabolic syndrome.
- The higher the numbers for HDL for both males and females, the more likely a patient does not develop metabolic syndrome.

## Model

Describe your final model

Report the most important metrics

Refer to the metrics to describe how well the model would solve the business problem

## Recommendations:

More of your own text here


## Limitations & Next Steps

More of your own text here


### For further information


For any additional questions, please contact:

Brooke Eagan
brooke.eagan4@gmail.com
