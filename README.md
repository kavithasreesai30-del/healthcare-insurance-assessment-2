![Code Institute Logo](https://codeinstitute.net/globalassets/images/logo.png)


# Healthcare Insurance Data Analysis — Advanced Analytics and Machine Learning

## Introduction

This project explores healthcare insurance costs using data analysis, statistical methods, data visualisation, and machine learning. The aim is to investigate how factors such as age, sex, body mass index (BMI), number of children, smoking status, and geographical region relate to insurance charges.

This project builds on the work completed in Unit 1 Assessment and extends the analysis through additional statistical investigation, machine learning model development and evaluation, and an interactive Tableau dashboard.

For Unit 2 Assessment, the project extends the original data analysis through further statistical investigation, data visualisation and machine learning. The data analysis findings are presented through visualisations and an interactive Tableau Public dashboard. Separately, Linear Regression and Random Forest Regression models are developed and evaluated to predict healthcare insurance charges.

## Acknowledgement of Previous Work

This project builds on the completed Unit 1 Assessment (Capstone Project), which explored healthcare insurance costs using the same dataset.

Relevant project files, data preparation and previous analysis were carried forward from Unit 1 as the starting point for further development. The Unit 2 Assessment extends this work through additional statistical analysis, visualisations and machine learning.

The original Unit 1 Assessment repository is available here: [Healthcare Insurance Cost Analysis – Assessment 1](https://github.com/kavithasreesai30-del/healthcare-insurance-capstone).

## Project Structure

The project is organised into folders to separate the source data, analysis notebook and project documentation.

```text
Healthcare_Insurance_Assessment2/
│
├── .github/
│
├── data/
│   ├── insurance.csv
│   └── insurance_cleaned.csv
│
├── notebooks/
│   ├── healthcare_insurance_analysis.ipynb
│   └── age_insurance_smoking_plot.html
│
├── README.md
├── requirements.txt
└── .gitignore


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

The project follows a structured data analysis workflow, building on the work completed in Unit 1 Assessment.

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

## Analysis Techniques and Limitations

### Analysis Techniques

The project uses a combination of data analysis, statistical methods, data visualisation and machine learning.

- **Data cleaning:** pandas is used to inspect the dataset, check for missing values and duplicate records, and prepare the data for analysis.
- **Exploratory data analysis:** descriptive statistics are used to summarise the dataset and understand the characteristics of the individuals and their insurance charges.
- **Statistical analysis:** group comparisons and correlation analysis are used to investigate patterns and relationships between insurance charges and individual characteristics.
- **Data visualisation:** Matplotlib and Plotly are used to explore and communicate patterns in the data through charts.
- **Machine learning:** Linear Regression and Random Forest Regression are trained to predict insurance charges. Their performance is compared using Mean Absolute Error (MAE), Root Mean Squared Error (RMSE) and R².
- **Interactive dashboard:** Tableau is used to present the findings through interactive visualisations and filters.

### Limitations and Alternative Approaches

The dataset contains a limited set of personal characteristics and insurance charges. Other factors that may influence insurance costs are not included, so the findings cannot explain every difference in charges.

The dataset is observational. Relationships identified through statistical analysis and visualisation do not establish that one characteristic directly causes changes in insurance charges.

Linear Regression provides a straightforward baseline model but may not capture complex, non-linear relationships. Random Forest Regression can model more complex patterns, although its predictions are less straightforward to interpret. Comparing both models helps assess their relative predictive performance.

Alternative approaches could include testing additional models, using further relevant data, and applying additional model interpretation techniques. These could be explored as future improvements if time and resources allow.

## Ethical Considerations

This project uses a publicly available healthcare insurance dataset for educational purposes. The analysis focuses on patterns in insurance charges and does not attempt to identify individuals.

The results show associations and predictive patterns, not proof that personal characteristics directly cause higher insurance charges. Factors such as age, sex, BMI and smoking status should be interpreted carefully to avoid unfair assumptions about individuals.

The machine learning models are intended for educational analysis and should not be used as the sole basis for real-world insurance decisions.

## Dashboard Design

In my project, I have used Tableau Public to create an interactive dashboard that presents the key findings from my healthcare insurance data analysis. The dashboard brings together six visualisations to help users explore the factors associated with medical insurance charges.

My aim was to present the findings in a clear and accessible way so that both technical and non-technical audiences can understand the results and explore patterns within the dataset.

### Dashboard Visualisations

I selected six visualisations to investigate different aspects of healthcare insurance charges:

- **Average Charges by Smoking Status:** This visualisation compares the average insurance charges of smokers and non-smokers, helping users explore the relationship between smoking status and insurance costs.

- **Charges Distribution by Smoking Status:** This box plot compares the distribution of charges for smokers and non-smokers, showing differences in the spread of charges and highlighting potential outliers.

- **Average Charges by Region:** This visualisation compares average insurance charges across the four geographical regions to identify differences between regional groups.

- **Average Charges by Region and Smoking Status:** This highlight table combines geographical region and smoking status to help users compare average charges across different groups.

- **BMI vs Insurance Charges:** This scatter plot explores the relationship between Body Mass Index (BMI) and insurance charges, helping users identify possible patterns in the data.

- **Age vs Insurance Charges:** This scatter plot explores the relationship between age and insurance charges, allowing users to examine how charges vary across different ages.

### Interactive Features

I have included interactive filters for region, smoking status and sex. These filters allow users to select particular groups and explore how the visualisations change according to their selections.

The interactive features encourage users to investigate the data independently rather than relying only on the initial charts. They also make it easier to compare groups and explore patterns relevant to the project questions.

### Communicating the Findings

The dashboard combines comparisons between groups, a box plot showing the distribution of charges, and scatter plots showing relationships between numerical variables. Each visualisation serves a specific purpose and contributes to a broader understanding of the factors associated with insurance costs.

By presenting the analysis through an interactive dashboard, I aim to make the findings easier to understand and explore. However, the patterns shown in the dashboard represent associations within the available dataset and do not establish that individual characteristics directly cause differences in insurance charges.

## Results and Evaluation

### Key Findings

The analysis identified differences in healthcare insurance charges across smoking status, age, BMI and geographical region.

The main findings include:

- **Smoking status:** Smokers had substantially higher average insurance charges than non-smokers in the dataset.
- **Age:** The visualisations helped explore how insurance charges vary with age.
- **BMI:** The analysis investigated the relationship between BMI and insurance charges.
- **Geographical region:** Comparing average charges across regions helped identify differences between regional groups.
- **Combined factors:** The highlight table allowed comparisons of average charges across geographical regions and smoking status.

These findings describe patterns in the available dataset and should not be interpreted as proof of cause and effect.

### Machine Learning Model Evaluation

I trained and evaluated two regression models to predict healthcare insurance charges: Linear Regression and Random Forest Regression.

The models were evaluated using Mean Absolute Error (MAE), Root Mean Squared Error (RMSE) and R².

| Evaluation Metric | Linear Regression | Random Forest Regression |
|---|---:|---:|
| MAE | 4,334.48 | 2,639.83 |
| RMSE | 6,023.86 | 4,673.26 |
| R² | 0.8025 | 0.8812 |

Lower MAE and RMSE values indicate smaller prediction errors, while a higher R² indicates that the model explains a greater proportion of the variation in the target variable.

Random Forest Regression performed better than Linear Regression across all three evaluation metrics. It produced lower prediction errors and a higher R² score on the test data.

### Overall Evaluation

The project combines exploratory data analysis, statistical investigation, visualisations and machine learning to examine healthcare insurance charges.

The Tableau dashboard communicates the findings interactively, while the regression models provide an additional way to investigate how individual characteristics can help predict insurance costs.

The results are limited by the variables available in the dataset and the performance of the models on the selected test data. The predictions should therefore be interpreted as estimates rather than exact insurance costs.

## Development Roadmap

### Challenges and Learning

During this project, I developed my skills in data cleaning, exploratory data analysis, statistical investigation, data visualisation and machine learning. I also gained experience in using Git and GitHub to manage project files and track development.

Comparing Linear Regression and Random Forest Regression helped me understand how different regression algorithms can perform when predicting insurance charges. Creating an interactive Tableau dashboard also helped me develop my skills in presenting analytical findings to different audiences.

### Future Improvements

Possible future improvements include:

- **Additional data:** Include more relevant variables that may help explain differences in insurance charges.
- **Model improvement:** Explore hyperparameter tuning and cross-validation to assess whether model performance can be improved.
- **Model interpretation:** Investigate additional techniques to understand which features contribute most to the models' predictions.
- **Dashboard development:** Refine the Tableau dashboard and its interactive features based on user feedback.
- **Further analysis:** Investigate additional statistical methods to explore relationships within the dataset.

These improvements could extend the analysis and support further development of my data analytics and machine learning skills.

## Main Data Analysis Libraries and Tools

The following tools and libraries were used to develop this project:

| Tool or Library | Purpose |
|---|---|
| Python | Main programming language used for data analysis and machine learning. |
| pandas | Used for data loading, cleaning, preparation and analysis. |
| NumPy | Used for numerical operations. |
| Matplotlib | Used to create data visualisations. |
| Plotly | Used to create interactive visualisations. |
| scikit-learn | Used to prepare data, train regression models and evaluate their performance. |
| Jupyter Notebook | Used to organise and document the analysis, code and findings. |
| Tableau Public | Used to create and publish the interactive dashboard. |
| Git and GitHub | Used for version control, project documentation and repository management. |
| Visual Studio Code | Used as the development environment for the project. |

## Credits and Acknowledgements

### Dataset

The healthcare insurance dataset was obtained from Kaggle:

- [Medical Cost Personal Datasets – Kaggle](https://www.kaggle.com/datasets/mirichoi0218/insurance)

### Previous Assessment Work

This project builds on my completed Unit 1 Assessment healthcare insurance analysis. Relevant files, data preparation and previous analysis were carried forward as the starting point for Unit 2 Assessment.

The original repository is available here:

- [Healthcare Insurance Cost Analysis – Assessment 1](https://github.com/kavithasreesai30-del/healthcare-insurance-capstone)

### Learning Resources and Documentation

The project was developed as part of the Code Institute Data Analytics and AI Bootcamp. Course materials, assessment guidance and official software documentation supported my learning and development.

Official documentation consulted includes resources for Python, pandas, Matplotlib, Plotly and scikit-learn. These resources help explain the tools and methods used in the project.

### Artificial Intelligence Assistance

I used ChatGPT and Claude as AI-assisted learning and development tools during this project. They supported my understanding of programming concepts, troubleshooting, code improvement, data analysis methods and project documentation.

AI-generated suggestions were used as assistance rather than a replacement for my own work. I reviewed and adapted suggestions to suit the project, and I remain responsible for the code, analysis, interpretation and final submitted work.

