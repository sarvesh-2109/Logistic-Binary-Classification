# Logistic Regression on HR Data

This repository contains a project that implements logistic regression to analyze and predict employee turnover using the HR dataset. The dataset includes various features such as satisfaction level, last evaluation, number of projects, average monthly hours, time spent at the company, work accidents, and promotions in the last five years.

## Project Overview

The main objectives of this project are:
- To understand the factors affecting employee turnover.
- To visualize the relationships between different features and employee turnover.
- To build a logistic regression model to predict whether an employee will leave the company.

## Dataset

The dataset used in this project is the HR dataset (`HR_comma_sep.csv`). It includes the following features:
- `satisfaction_level`
- `last_evaluation`
- `number_project`
- `average_montly_hours`
- `time_spend_company`
- `Work_accident`
- `promotion_last_5years`
- `Department`
- `salary`
- `left` (target variable indicating if the employee left the company)

## Libraries Used

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## Notebook Content

### 1. Data Import and Exploration

The dataset is loaded and basic statistics are displayed using `data.describe()`. The dataset is also inspected for any missing values and data types.

### 2. Data Preprocessing

- **Label Encoding**: The categorical variables `Department` and `salary` are encoded using `LabelEncoder`.
- **Correlation Matrix**: The correlation matrix is computed and visualized using a heatmap to understand the relationships between features and the target variable `left`.

### 3. Data Visualization

- Various box plots and count plots are created to visualize the relationships between different features and the target variable `left`.
- Plots include:
  - Satisfaction Level vs Left
  - Last Evaluation vs Left
  - Number of Projects vs Left
  - Average Monthly Hours vs Left
  - Time Spent at Company vs Left
  - Salary vs Left
  - Department vs Left
  - Work Accident vs Left
  - Promotion Last 5 Years vs Left

### 4. Feature Engineering

- **Dummy Variables**: Dummy variables are created for the `salary` feature and concatenated with the dataset.
- **Subsetting Features**: A subset of features is selected for model training, including `satisfaction_level`, `average_montly_hours`, `promotion_last_5years`, and dummy variables for `salary`.

### 5. Model Training and Evaluation

- **Train-Test Split**: The dataset is split into training and testing sets using `train_test_split`.
- **Logistic Regression**: A logistic regression model is trained using the training set.
- **Model Evaluation**:
  - Confusion Matrix
  - Classification Report
  - Accuracy Score

## Results

- The confusion matrix, classification report, and accuracy score are displayed to evaluate the performance of the logistic regression model.

## Visualizations

- Confusion Matrix: A heatmap of the confusion matrix is generated to visualize the model's performance.

## Conclusion

The logistic regression model provides insights into the factors affecting employee turnover and achieves a certain level of accuracy in predicting employee turnover.

## How to Run the Notebook

1. Clone the repository:
   ```bash
   git clone https://github.com/sarvesh-2109/Logistic-Binary-Classification.git
   cd Logistic-Binary-Classification
   ```

2. Install the required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```

3. Run the Jupyter notebook:
   ```bash
   jupyter notebook Logistic_Binary.ipynb
   ```

## Acknowledgements

- The dataset is sourced from the HR dataset available on Kaggle.
- This project was developed using the Jupyter notebook on Google Colab.

Feel free to explore and contribute to the project!
