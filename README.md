# UK Bank Campaign Analysis and Prediction

This project analyzes and predicts customer responses to a UK bank’s fixed-term savings account campaign using data-driven techniques. It involves preprocessing data, exploratory data analysis (EDA), and building machine learning models to assess campaign effectiveness and predict customer responses.

## Overview

The analysis is structured into two main objectives:
1. **Data Preprocessing and EDA**:
   - Cleaning and merging datasets.
   - Visualizing customer demographics, financial attributes, and campaign performance.
2. **Model Building and Evaluation**:
   - Developing classification models (Logistic Regression, Decision Tree, and KNN).
   - Comparing model performances using metrics such as accuracy, precision, recall, F1-score, and ROC-AUC.

## Project Highlights
- **Datasets**:
  - `all_campaign.csv`: Contains campaign-related information and responses.
  - `all_personal.csv`: Includes customer demographics and financial data.
- **Key Findings**:
  - Younger (18-30) and older (61-80) demographics respond better to campaigns.
  - Positive responses correlate with higher account balances and longer contact durations.
  - Decision Tree model outperforms others with an AUC of 0.84.

## Methodology

### Data Preprocessing
- Handled missing values by imputing the `education` column.
- Removed duplicates and irrelevant features.
- Merged datasets using the common `custID` column.

### Exploratory Data Analysis (EDA)
- Visualized response rates by age, marital status, region, and education.
- Analyzed correlations between variables like balance, duration, and responses.

### Model Development
1. **Logistic Regression**: Basic linear model with good overall accuracy but struggled with minority class predictions.
2. **Decision Tree**: Best-performing model, offering high interpretability and balanced precision-recall metrics.
3. **K-Nearest Neighbors (KNN)**: Effective for majority class but less accurate for minority predictions.

### Evaluation Metrics
- **Accuracy**: Measures overall correctness of predictions.
- **Precision and Recall**: Focus on minority class (`yes`) predictions.
- **ROC-AUC**: Evaluates model discrimination ability.

## Key Visualizations
- **Response Rates by Age Group**: Highlights demographic-specific engagement.
- **ROC Curves**: Compare model performances.
- **Correlation Heatmap**: Show relationships between key variables.

## Recommendations
- Utilize the Decision Tree model for future campaigns.
- Focus marketing efforts on high-response demographics and regions.
- Integrate transaction data and seasonal trends for improved targeting.

## Dependencies
- Python libraries:
  - `pandas`, `numpy`: Data manipulation.
  - `matplotlib`, `seaborn`: Visualization.
  - `scikit-learn`: Model building and evaluation.

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/MuhammadHamza1487/UK-Bank-Compaign.git
   ```
3. Run the Jupyter Notebook for full analysis:
   ```bash
   main.ipynb
   ```
