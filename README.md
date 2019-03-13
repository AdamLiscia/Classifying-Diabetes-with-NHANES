# Classifying Diabetes with NHANES

Classifying whether someone is diabetic, prediabetic, or healthy with the NHANES database.

# Why diabetes?
* It costs a lot:
  * $327 billion: Total costs of diagnosed diabetes in the United States in 2017
  * $237 billion for direct medical costs
  * $90 billion in reduced productivity
* 7th leading cause of death
* 30.3 million Americans, or 9.4% of the population
* 1.5 million Americans are diagnosed with diabetes every year
* In 2015, 84.1 million Americans age 18 and older had prediabetes
* http://www.diabetes.org/diabetes-basics/statistics/

***

# About NHANES
* Conducted by the Centers for Disease Control and Prevention every 2 years
* 15,327 persons were selected for NHANES from 30 different survey locations
* 9,971 people  completed the interview
* 9,544 people were examined
* Represents all age groups
* Over samples minority groupsto produce reliable statistics


##### The NHANES dataset has 5 main components:
* Demographics
* Dietary
* Examination
* Questionnaire
* Laboratory

### Demographics
* Age
* Gender
* Education
* Income
* Race
* Citizenship
* Language
* Family Size

### Dietary
* 2 Days
* Macronutrients
* Micronutrients
* Water
* Caffeine
* Alcohol

### Examination
* Body Measurements
  * Weight
  * Height
  * BMI
  * Waist Circumference
* Blood Pressure
  * Resting Heart Rate
  * Systolic
  * Diastolic

### Questionnaire
* Lifestyles and Habits
* Physical Activity
* Weight History
* Tobacco Use
* Health Insurance
* Occupations
* Sleep Quality
* Consumer Habits
* Transportation
* Where do you buy your food?

### Laboratory
* Bloodwork Data
* Why I’m not using this:
  * These are the numbers used to determine diabetes
  * I would like to be able to predict without it
  * It would feel like cheating to use these

***

# The Process
* This project can be broken down into the following steps:
  * Obtained the data from the CDC
  * Exploratory Data Analysis
  * Cleaned with Pandas
  * Train - Test - Split
  * SMOTE of downsample the training set
  * Pipeline and GridSearchCV to find the best models
  * Look into the evaluation metrics
  
### Libraries Used
* Pandas
* Numpy
* MatPlotLib
* Seaborn
* SciKit Learn
* SMOTE
* Pipeline
* GridSearchCV
  

***

# Current Best Model
* No Scaling
* SMOTE
* Random Forest Classifier
* 69.6% Accuracy

# Next Steps
* Feature Selection and Feature Engineering
* Need to remove noise and overfitting
* Change my target to heart disease
* Changes I know I want to make:
    * Remove everyone older than 79
    * Remove micro nutrients
    * Remove head of household columns

# It will never be perfect, somethings are just out of your control
* The human body is very complex and everybody is different
* Measure Bias will always be an issure
* Healthy User Bias
* Recall Bias
