# Credit Card Approval Status: Classification

**Author:** Neeraj Kumar Paikra
#### Detail Documentation: https://docs.google.com/document/d/1FUs_6PuCMFm6Ii-w1EdNe4py8zTwFFyAWn_kmGUcKDM/edit?usp=sharing
#### SQL Questions: https://docs.google.com/document/d/1Pjo4JslsjsWge7FSE03BujS1fDgU0RTwrthhDSjaOmY/edit?usp=sharing

![68747470733a2f2f7777772e6361726472617465732e636f6d2f77702d636f6e74656e742f75706c6f6164732f323032302f30382f7368757474657273746f636b5f3537363939383233302e6a7067](https://github.com/Npps1997/Credit-Card-Approval-Prediction-Classification/assets/96871890/08831849-a3be-433f-8f9f-ef831f55dee6)



## Overview
This GitHub repository contains code and documentation for a credit card approval status classification project. The project aims to predict whether a credit card application will be approved or declined based on various factors and criteria provided in the dataset.

## Key Points
- **Importance of the Project**:

| Key Point                                     | Description                                                                                               |
|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------|
| Helping More People Get Credit                | More individuals, even with imperfect financial histories, gain access to credit cards.                |
| Strengthening the Economy                    | Responsible lending prevents economic instability, fosters investment, growth, and job opportunities.    |
| Keeping People Safe from Bad Loans           | Safeguards against unaffordable loans and prevents individuals from falling into a cycle of debt.        |
| Protecting Banks from Losing Money           | Helps banks make informed lending decisions to minimize financial losses.                                   |
| Fairness and No Discrimination               | Ensures equal opportunities for all applicants, regardless of background.                                  |
| Using Technology Wisely                      | Advanced technology like AI streamlines the credit card approval process for better decisions.           |

- **Impact on the Banking Sector**:

| Impact                                       | Description                                                                                               |
|----------------------------------------------|-----------------------------------------------------------------------------------------------------------|
| Less Risk, More Money                        | Banks can avoid risky clients, ensuring financial stability and increased profits.                       |
| Happy Customers                              | Faster credit card approvals lead to happier customers who are likely to use more banking services.      |
| Cost Savings                                 | Efficient resource utilization saves money on debt collection.                                            |
| Competitive Advantage                        | Attracts responsible customers and informs strategic decisions.                                            |

- **Gap in Knowledge**:

| Knowledge Gap                              | Description                                                                                                |
|--------------------------------------------|------------------------------------------------------------------------------------------------------------|
| Assisting Indian Banks                     | The project's methodology can be applied to Indian banks in the future.                                     |
| Understanding Indian Customers             | The model can adapt to Indian customer behavior.                                                             |
| Supporting More People                     | Facilitates access to banking services for a broader population.                                              |
| Risk Mitigation                            | Helps Indian banks avoid financial losses.                                                                  |

## Project Details

### Introduction
- **Goal**: Create a classification model for credit card approval status.
- **Objectives**:
  - Develop an accurate prediction model.
  - Identify influential approval factors.
  - Provide insights for informed lending decisions.

### Dataset
- **Features**: Various client attributes (e.g., income, education, gender).
- **Label**: Approval status (0 for approved, 1 for rejected).

### Approach
1. **Exploratory Data Analysis (EDA)**:

| EDA Aspect                        | Description                                                                                         |
|-----------------------------------|-----------------------------------------------------------------------------------------------------|
| Analyze Feature Distributions     | Understand the distribution of features in the dataset.                                            |
| Visualize Feature-Target Relationships | Explore how features relate to the approval status.                                              |

2. **Data Preprocessing**:

| Preprocessing Task                | Description                                                                                         |
|-----------------------------------|-----------------------------------------------------------------------------------------------------|
| Handle Missing Values             | Address missing data in the dataset.                                                               |
| Outlier Handling                   | Identify and manage outliers in the data.                                                          |
| Feature Engineering                | Create new features if necessary and encode categorical variables.                                    |

3. **Model Selection**:
   - Evaluate multiple classification algorithms (e.g., XGBoost, Random Forest).
   - Optimize models using hyperparameter tuning.

4. **Feature Importance Analysis**:
   - Determine key features influencing approval decisions.

5. **Model Evaluation**:
   - Assess model performance on test data.
   - Choose the best-performing model.

### Results

#### Feature Selection and Model Performance

| Sr. No. | Feature Selection       | Best Algorithm      | Performance Metric | Score   |
|---------|-------------------------|----------------------|--------------------|---------|
| 1       | Without Feature Selection | Random Forest, XGBoost | Recall             | 96      |
| 2       | Logistic L1 Lasso        | XGBoost              | Recall             | 95.6    |
| 3       | Logistic L2 Ridge        | XGBoost              | Recall             | 92.3    |
| 4       | LDA                       | XGBoost              | Precision          | 89.1    |
| 5       | PCA                       | Gradient Boosting    | Recall             | 84.3    |
| 6       | XGBoost (Imbalanced data) | Random Forest        | Accuracy, Recall   | 94      |
| 7       | XGBoost (Balanced data)   | XGBoost              | All                | 94-95   |


- **XGBoost** outperformed other models with accuracy, precision, recall, and F1-score ranging from 94% to 95%.
- Addressing class imbalance improved model performance.

## Recommendations
- **Data Resampling**: Consider oversampling or undersampling to address class imbalance.
- **Feature Selection and Engineering**: Continue exploring relevant features.
- **Hyperparameter Tuning**: Optimize model hyperparameters.
- **Evaluate More Models**: Experiment with other classification algorithms.
- **Collect More Data**: Enhance model training with additional data.

For detailed code and analysis, please refer to the project's Jupyter Notebook (`CAPSTONE_(Credit_Card_Approval_Classification).ipynb`).

## Dependencies
- Jupyter Notebook
- Scikit-Learn
- Python

## Additional Information
For SQL-related questions related to this project, please refer to the 'https://docs.google.com/document/d/1Pjo4JslsjsWge7FSE03BujS1fDgU0RTwrthhDSjaOmY/edit?usp=sharing' section.

Feel free to reach out for further details or collaboration opportunities.

**Thank you for exploring this project!**

