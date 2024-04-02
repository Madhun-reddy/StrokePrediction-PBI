# Stroke Prediction using Power BI
According to the World Health Organization (WHO) stroke is the 2nd leading cause of death globally, responsible for approximately 11% of total deaths.
This dataset is used to predict whether a patient is likely to get stroke based on the input parameters like gender, age, various diseases, and smoking status. Each row in the data provides relavant information about the patient.

## Dataset
The dataset used in this project consists of 5110 observations with 12 attributes, including information on demographics, medical history, lifestyle factors, and stroke occurrence. The dataset was carefully prepared and explored, including handling missing values, performing descriptive statistics, and visualizing the data distribution.

## Descriptor Information
1) id: unique identifier
2) gender: "Male", "Female" or "Other"
3) age: age of the patient
4) hypertension: 0 if the patient doesn't have hypertension, 1 if the patient has hypertension
5) heart_disease: 0 if the patient doesn't have any heart diseases, 1 if the patient has a heart disease
6) ever_married: "No" or "Yes"
7) work_type: "children", "Govt_jov", "Never_worked", "Private" or "Self-employed"
8) Residence_type: "Rural" or "Urban"
9) avg_glucose_level: average glucose level in blood
10) bmi: body mass index
11) smoking_status: "formerly smoked", "never smoked", "smokes" or "Unknown"*
12) stroke: 1 if the patient had a stroke or 0 if not
*Note: "Unknown" in smoking_status means that the information is unavailable for this patient

## Data Preparation and Exploration
The data preprocessing phase involved removing unnecessary columns, addressing missing values, categorizing features, and standardizing the data. Exploratory data analysis was conducted to gain insights into the dataset, including visualizations of categorical and numerical columns, identifying outliers, and examining correlations among variables.

## Univariate Analysis
Univariate analysis focuses on analyzing one variable at a time. Let’s explore the insights from a univariate perspective based on the provided data

## Bivariate Analysis
Bivariate analysis focuses on analyzing any concurrent relation between two variables or attributes. Let’s explore the insights from a bivariate perspective based on the provided data

### Stroke occurrences based on Age high risk group(individual age >55 group as high risk):

**1.	Age High Risk and Stroke:**

**High-Risk Age Group:**
-	Individuals aged greater than 55 are considered high-risk.
-	This group includes 206 individuals who have experienced a stroke.
-	They account for 82.73% of all stroke cases in the dataset.

**Low-Risk Age Group:**
-	Individuals aged below 55 fall into the low-risk category.
-	Only 43 individuals in this group have had a stroke.
-	They represent 17.27% of stroke cases.

**Implications:**
-	The high-risk age segment faces a significantly higher risk of stroke.
-	Organizations and healthcare providers should focus on preventive measures and early detection for this demographic.
-	Lifestyle modifications, regular health check-ups, and awareness campaigns can help mitigate stroke risk.

### Stroke occurrences based on marital status

**2.	Marital Status and Stroke:**
The dataset includes individuals categorized by their marital status: unspecified (NA), currently married (Yes), and never married (No).

The raw numbers indicate the following:
-	Never married (NA):
  -	25 individuals had a stroke.
  -	1753 individuals did not have a stroke.

-	Currently married (Yes):
  -	203 individuals had a stroke.
  -	3336 individuals did not have a stroke.
- The total sample size is 5110 individuals.
-	21 individuals who had stroke are from unspecified (NA) group

### Stroke occurrences based on Gender

**3.	Gender and Stroke:**
The dataset includes individuals categorized by gender: Female, Male, NA (Not Available), and Other.

The raw numbers indicate the following:

**Females:**
-	132 individuals had a stroke.
-	2985 individuals did not have a stroke.

**Males:**
-	106 individuals had a stroke.
-	2113 individuals did not have a stroke.

### Stroke occurrences based on different job types

**4.	Job Types and Stroke:**
The dataset includes individuals categorized by their job types: children, government jobs, NA (not available), never worked, private jobs, and self-employed.

The raw numbers indicate the following:

- Private jobs:
  -  2776 individuals did not have a stroke.
  -  145 individuals had a stroke.

- Self-employed:
  -  54 individuals did not have a stroke.
  -  64 individuals had a stroke.


## Insights:
1.	The high-risk age segment faces a significantly higher risk of stroke.
2.	Organizations and healthcare providers should focus on preventive measures and early detection for this demographic.
3.	Lifestyle modifications, regular health check-ups, and awareness campaigns can help mitigate stroke risk.
4.	Marital status appears to be associated with stroke risk.
5.	Individuals who are currently married have over 81% higher likelihood of experiencing a stroke compared to those who are never married is 10%.
6.	Females have a slightly higher likelihood of experiencing a stroke compared to males.
7.	Job type may play a role in stroke prediction. So individuals in private jobs  had over 58% and those who are self-employed had 26% stroke and appear to have a slightly higher likelihood of experiencing a stroke in these categories of workers.


## Category vs Target Analysis
Let’s analyze the insights and recommendations based on different categories compared to the target:

1.	Gender:

-	Female: 4.42% stroke rate.
-	Male: 5.02% stroke rate.
-	Other: 0.00% stroke rate.
-	Overall: 4.87% stroke rate.

**Recommendation:** Focus on preventive measures for both genders, with special attention to males.

2.	Marital Status:

-	Ever married: 6.09% stroke rate.
-	Never married: 1.43% stroke rate.
-	Overall: 4.87% stroke rate.

**Recommendation:** Prioritize preventive strategies for ever-married individuals.

3.	Residence Type:

- Urban: 5.09% stroke rate.
-	Rural: 4.42% stroke rate.
-	Overall: 4.87% stroke rate.

**Recommendation:** Address urban lifestyle factors to reduce stroke risk.

5.	Age Risk:

-	High Risk Age (>55): 12% stroke rate.
-	Low Risk Age: 1% stroke rate.

**Recommendation:** Target health interventions for older populations.

6.	High-Risk Factors:
   
- Individuals with high-risk factors have a significantly higher stroke rate.

**Recommendation:** Identify and mitigate these factors proactively.

7.	Heart Disease:
   
-	Individuals with heart disease face an extremely high stroke risk.

**Recommendation:** Manage and prevent heart diseases rigorously.

8.	Hypertension:
   
-	Hypertension significantly increases stroke risk.

**Recommendation:** Control blood pressure effectively.


## Continuous vs Target Analysis

**Continuous Variables Insights**
-	Age: Individuals who have had a stroke tend to be older on average.
-	BMI: There is a slight increase in average BMI for individuals who have had a stroke.
-	Glucose Level: Individuals with higher average glucose levels seem more prone to strokes.

**Recommendations:**
-	Age: Focus preventive measures on older adults as they are at higher risk.
-	BMI: Monitor and manage BMI to mitigate stroke risk.
-	Glucose Level: Control blood glucose levels effectively.

## Conclusion and Recommendations
The results demonstrated that our models achieved high recall for stroke cases despite the imbalanced nature of the dataset. Age was found to be a significant predictor, along with other features such as smoking status and work type. The developed model can serve as a valuable tool in identifying individuals at risk of stroke and implementing preventive interventions.

Further analysis and exploration are recommended to delve deeper into genetic factors, long-term effects of lifestyle modifications, advanced predictive models, socioeconomic and cultural factors, novel biomarkers, imaging techniques, and personalized stroke prevention strategies.
