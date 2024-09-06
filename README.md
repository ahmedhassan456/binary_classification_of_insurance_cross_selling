# Insurance Cross-Selling Prediction

## Project Overview

This project aims to predict which customers are more likely to respond positively to an automobile insurance offer. Using a dataset with customer and vehicle information, we apply machine learning techniques to classify customers' responses.

## Dataset Description

The dataset contains the following features:

- **Gender**: Categorical variable indicating the customer's gender.
- **Age**: Numeric variable indicating the age of the customer.
- **Driving_License**: Binary variable indicating if the customer holds a driving license (1 = Yes, 0 = No).
- **Region_Code**: Numeric variable representing the region code of the customer.
- **Previously_Insured**: Binary variable indicating if the customer already has an insurance policy (1 = Yes, 0 = No).
- **Vehicle_Age**: Categorical variable representing the age of the vehicle (e.g., "< 1 Year", "1-2 Year", "> 2 Years").
- **Vehicle_Damage**: Categorical variable indicating if the customer’s vehicle has been damaged in the past ("Yes", "No").
- **Annual_Premium**: Numeric variable showing the annual premium paid by the customer.
- **Policy_Sales_Channel**: Numeric variable representing the sales channel through which the policy was sold.
- **Vintage**: Numeric variable showing the number of days the customer has been associated with the insurance company.
- **Response**: Binary target variable where 1 indicates that the customer responded positively to the offer, and 0 indicates otherwise.

## Project Workflow

1. **Data Preprocessing**:
   - Handle missing data (if any).
   - Encode categorical variables (e.g., `Gender`, `Vehicle_Age`, `Vehicle_Damage`).
   - Feature scaling for numeric columns (e.g., `Annual_Premium`, `Age`, `Vintage`).

2. **Exploratory Data Analysis (EDA)**:
   - Visualize the distribution of features.
   - Analyze the relationships between different features and the target variable (`Response`).

3. **Modeling**:
   - Multiple machine learning algorithms were tested, including:
     - Logistic Regression
     - Decision Trees
     - Random Forests
     - Gradient Boosting Machines (GBM)
     - XGBoost
   - Hyperparameter tuning was performed using grid search or randomized search to optimize the model.

4. **Model Evaluation**:
   - Performance metrics used include:
     - Accuracy
     - Precision
     - Recall
     - F1 Score
     - ROC-AUC curve

5. **Deployment**:
   - The model is deployed using a web framework (e.g., Streamlit, Flask, FastAPI).

## Getting Started

### Prerequisites

To run this project, ensure you have the following dependencies installed:

- Python 3.x
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn
- xgboost
- Streamlit (optional, for deployment)


## Future Improvements

- Fine-tuning the model with additional hyperparameter optimization techniques.
- Incorporating more advanced feature engineering methods.
- Testing additional machine learning models (e.g., LightGBM, CatBoost).

## License

This project is licensed under the MIT License.
