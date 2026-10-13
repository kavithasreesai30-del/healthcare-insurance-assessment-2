![Code Institute Logo](https://codeinstitute.net/globalassets/images/logo.png)


# Healthcare Insurance Data Analysis — Advanced Analytics and Machine Learning

## Introduction

This project explores healthcare insurance costs using data analysis, statistical methods, data visualisation, and machine learning. The aim is to investigate how factors such as age, sex, body mass index (BMI), number of children, smoking status, and geographical region relate to insurance charges.

This project builds on the work completed in Unit Assessment 1 and extends the analysis through additional statistical investigation, machine learning model development and evaluation, and an interactive Tableau dashboard.

The original Unit Assessment 1 project is available here: [Healthcare Insurance Cost Analysis – Assessment 1](https://github.com/kavithasreesai30-del/healthcare-insurance-capstone).

For Unit Assessment 2, the project compares Linear Regression and Random Forest Regression models to predict insurance charges. The findings are communicated through data visualisations and an interactive Tableau dashboard.

## Acknowledgement of Previous Work

This project builds on the completed Unit 1 Assessment (Capstone Project), which explored healthcare insurance costs using the same dataset.

Relevant project files, data preparation and previous analysis were carried forward from Unit 1 as the starting point for further development. The Unit 2 Assessment extends this work through additional statistical analysis, visualisations and machine learning.

The original Unit 1 Assessment repository is available here: [Healthcare Insurance Cost Analysis – Assessment 1](https://github.com/kavithasreesai30-del/healthcare-insurance-capstone).

## Dataset Content

The project uses the [Medical Cost Personal Datasets from Kaggle](https://www.kaggle.com/datasets/mirichoi0218/insurance), which contains information about individuals and their medical insurance charges. The dataset is provided in CSV format.

The original dataset contains 1,338 records and seven columns:

| Column | Description |
|---|---|
| `age` | Age of the individual in years. |
| `sex` | Sex of the individual, recorded as female or male. |
| `bmi` | Body Mass Index (BMI), a measure relating weight to height. |
| `children` | Number of children covered by the insurance policy. |
| `smoker` | Smoking status, recorded as yes or no. |
| `region` | Geographical region of the individual, recorded as northeast, northwest, southeast or southwest. |
| `charges` | Individual medical insurance charges. |

The dataset supports the investigation of relationships between personal characteristics, smoking status, geographical region and medical insurance charges.

## Business Requirements

The project aims to investigate the factors associated with healthcare insurance charges and use data analysis to support a better understanding of variations in insurance costs.

The main business requirements are:

- Investigate how smoking status relates to average healthcare insurance charges.
- Examine the relationship between age and insurance charges.
- Investigate the relationship between Body Mass Index (BMI) and insurance charges.
- Compare average insurance charges across geographical regions.
- Explore whether the relationship between smoking status and insurance charges varies across regions.
- Develop and evaluate machine learning models to predict insurance charges using the available individual characteristics.
- Present key findings through clear data visualisations and an interactive Tableau dashboard.

## Hypotheses and Validation

The following hypotheses guide the investigation of healthcare insurance charges. They are explored using statistical analysis, data visualisations and machine learning.

| Hypothesis | Validation Method |
|---|---|
| Smokers have higher average insurance charges than non-smokers. | Compare average charges by smoking status and examine the distribution of charges using a box plot. |
| Insurance charges tend to increase with age. | Use a scatter plot to explore the relationship between age and insurance charges. |
| BMI is associated with insurance charges. | Use a scatter plot to investigate the relationship between BMI and insurance charges. |
| Average insurance charges vary across geographical regions. | Compare average charges by region using data visualisation. |
| The relationship between smoking status and insurance charges varies across regions. | Compare average charges by region and smoking status using a highlight table. |
| Machine learning can be used to predict insurance charges from individual characteristics. | Train and evaluate Linear Regression and Random Forest Regression models using MAE, RMSE and R². |

These hypotheses are investigated using the available dataset. The results identify associations and predictive patterns; they do not establish that a particular characteristic directly causes higher insurance charges.

## Project Plan

The project follows a structured data analysis workflow, building on the work completed in Unit Assessment 1.

### Project Stages

1. **Project setup:** Organise the repository, establish the project structure and prepare the Python environment.
2. **Data collection:** Use the Medical Cost Personal Datasets from Kaggle and retain the original dataset.
3. **Data cleaning and preparation:** Inspect data types, check for missing values and duplicate records, remove the duplicate record, and prepare a cleaned dataset for analysis.
4. **Exploratory data analysis:** Use descriptive statistics and visualisations to understand the dataset and investigate patterns in insurance charges.
5. **Statistical analysis:** Examine relationships between insurance charges and individual characteristics, including age, BMI, smoking status and geographical region.
6. **Machine learning:** Train and evaluate Linear Regression and Random Forest Regression models to predict insurance charges.
7. **Dashboard development:** Create an interactive Tableau dashboard to communicate the main findings.
8. **Evaluation and documentation:** Interpret the results, assess the limitations of the analysis and document the project in the notebook and README.

### Data Management and Methodology

The original CSV file is retained as the raw dataset. A cleaned version is prepared for analysis to preserve the original data and make the cleaning process transparent.

Python and pandas are used for data inspection, cleaning and preparation. Statistical analysis and visualisations are used to investigate patterns and relationships. Linear Regression and Random Forest Regression are compared using Mean Absolute Error (MAE), Root Mean Squared Error (RMSE) and the coefficient of determination (R²).

Tableau is used to present the findings in an interactive dashboard. This combination of methods supports both detailed analysis and accessible communication of the results.

## Rationale for Data Visualisations

The visualisations were selected to help investigate the project hypotheses and communicate patterns in healthcare insurance charges.

| Visualisation | Purpose |
|---|---|
| Average Charges by Smoking Status | Compare average insurance charges for smokers and non-smokers. |
| Charges Distribution by Smoking Status (Box Plot) | Examine the distribution of charges and identify differences between smokers and non-smokers. |
| Average Charges by Region | Compare average insurance charges across geographical regions. |
| Average Charges by Region and Smoking Status (Highlight Table) | Explore differences in average charges by region and smoking status. |
| BMI vs Insurance Charges (Scatter Plot) | Investigate the relationship between BMI and insurance charges. |
| Age vs Insurance Charges (Scatter Plot) | Investigate the relationship between age and insurance charges. |

These visualisations were chosen because they support comparisons between groups, show the distribution of charges and help explore relationships between numerical variables. Together, they provide evidence to help answer the project questions and communicate findings to different audiences.

The interactive Tableau dashboard includes filters for region, smoking status and sex, allowing users to explore selected groups within the dataset.




