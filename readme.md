# A Comparative Study for Machine Learning Models for Predicting Obesity

## Overview

This project is part of the Master of Data Science program and focuses on using machine learning techniques to predict obesity levels based on lifestyle and demographic data. The study compares three machine learning algorithms: **Logistic Regression**, **Decision Tree Classifier**, and **Random Forest D**.


### Course:
PRT565: Machine Learning and Artificial Intelligence  
Charles Darwin University, Sydney Campus

## Problem Description

Obesity is a significant global health issue, contributing to several noncommunicable diseases (NCDs) such as cardiovascular disease, type 2 diabetes, and certain types of cancer. This project aims to predict obesity levels using machine learning models based on individual lifestyle and demographic attributes. Accurate predictions can help in early intervention and healthcare planning.

## Dataset Description

The dataset used contains 17 attributes related to individuals' eating habits, physical conditions, and demographic data. The key features include:
- **Age**: Age of the individual.
- **Height**: Height in meters.
- **Weight**: Weight in kilograms.
- **favc**: Frequency of high-calorie food consumption.
- **ncp**: Number of meals per day.
- **caec**: Eating habits between meals.
- **nobeyesdad**: Obesity level (target variable).

More information on the dataset can be found at [UCI Machine Learning Repository](https://doi.org/10.24432/C5H31Z).

## Choice of Algorithms

Three machine learning algorithms were selected for comparison:
1. **Logistic Regression**: A simple and effective baseline model for classification tasks.
2. **Decision Tree Classifier**: Ideal for capturing non-linear relationships between features.
3. **Random Forest Classifier**: An ensemble technique that enhances model robustness and accuracy by combining multiple decision trees.

## Key Steps in the Process

1. **Data Understanding**: 
   - The dataset was inspected using methods such as `head()`, `info()`, and `describe()` to get a sense of the structure and data types.
   
2. **Data Pre-processing**:
   - Missing values were handled, and categorical features were encoded using One-Hot Encoding.
   - Outliers were detected using the IQR method and capped to prevent skewing model results.
   
3. **Exploratory Data Analysis (EDA)**:
   - Numeric and categorical features were visualized to understand distributions and relationships.
   - Correlation analysis was conducted to identify relationships between features.
   
4. **Model Building**:
   - Each algorithm was trained and tested using a 70/30 train-test split.
   - Pipelines were constructed for each model to streamline preprocessing and training steps.

## Results

- **Logistic Regression** achieved an accuracy of 85.01% on the test set, serving as a baseline.
- **Decision Tree Classifier**: The highest accuracy was 94.10%, achieved with a maximum tree depth of 9.
- **Random Forest Classifier**: Outperformed other models with an accuracy of 95.22% at a max depth of 10. Feature importance analysis showed that weight and family history of obesity were the most significant predictors.

## Conclusion

The study demonstrated that ensemble models like Random Forest provide better accuracy and stability compared to simpler models like Logistic Regression and Decision Trees. Random Forest's ability to handle complex feature interactions makes it the best choice for this dataset, achieving an accuracy of 95.22%.

## References

- [UCI Machine Learning Repository: Estimation of Obesity Levels Based on Eating Habits and Physical Condition](https://doi.org/10.24432/C5H31Z)
- [World Health Organization - Obesity and Overweight](https://www.who.int/news-room/fact-sheets/detail/obesity-and-overweight)
- [World Obesity Federation - World Obesity Atlas 2022](https://www.worldobesity.org/resources/resource-library/world-obesity-atlas-2022)
