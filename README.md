# linear-regression-data
🚢 Titanic Dataset: Linear Regression Model on Fare Prediction
📊 Project Overview
This project applies Linear Regression to predict the Fare of passengers aboard the Titanic based on selected features from the dataset. The goal is to create a regression model that can approximate the relationship between input features and the actual fare.

📁 Dataset
File Used: titanic dataset.csv

Source: Kaggle Titanic Dataset

Target Variable: Fare

Possible Features Used: May include Pclass, Age, SibSp, Parch, Sex, Embarked (though the exact features used are not visible in the screenshot).

🧠 Model Used
Algorithm: LinearRegression() from sklearn.linear_model

Evaluation Metrics:

MAE (Mean Absolute Error): 27.54

MSE (Mean Squared Error): 1709.21

R² Score: 0.4987

🔍 Interpretation:

An R² score of 0.4987 indicates that the model explains approximately 49.87% of the variance in the target variable.

The high MSE suggests some outliers or a wide variance in prediction.

📈 Graph: Actual vs Predicted Fare
Type: Scatter Plot

X-Axis: Actual Fare

Y-Axis: Predicted Fare

Diagonal Line: Red dashed line (y = x) represents perfect predictions — where predicted values equal actual values.

Observations:

Many data points fall below the red line, indicating underprediction.

The spread increases for higher fare values, which is common in datasets with skewed distributions.

Outliers are visible — for example, actual fares > 200 but predicted much lower.

🔍 Model Limitations
The regression model struggles with higher fare values, indicating possible non-linearity or missing key features.

Feature scaling and transformation might improve performance.

Outliers may heavily influence the model — a robust regression or log transformation of Fare could help.

📌 Next Steps
Apply feature engineering:

Encode categorical variables (Sex, Embarked)

Impute missing values

Normalize or scale features

Try different algorithms:

Ridge, Lasso, or RandomForestRegressor

Tune hyperparameters using GridSearchCV or RandomizedSearchCV

Perform log transformation on Fare to reduce skewness

📦 Requirements
bash
Copy
Edit
pip install pandas matplotlib scikit-learn seaborn
▶️ How to Run
Upload titanic dataset.csv to your Colab session.

Run all cells in the notebook.

Visual output including metrics and scatter plot will be displayed.
