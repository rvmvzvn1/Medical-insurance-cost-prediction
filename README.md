# Medical-insurance-cost-prediction
Machine learning project for predicting medical insurance costs using Linear Regression and ElasticNet, with data preprocessing, One-Hot Encoding, feature scaling, and model evaluation.

# Medical Insurance Cost Prediction

This is my second Machine Learning project.

The goal of this project is to predict medical insurance costs based on personal information such as age, BMI, number of children, smoking status, sex, and region.

I used this project to practice the complete workflow of a regression problem and compare different linear models.

# Dataset

The dataset contains information about medical insurance customers.

Features:

- `age` — age of the customer
- `sex` — sex of the customer
- `bmi` — body mass index
- `children` — number of children
- `smoker` — smoking status
- `region` — customer's region

Target:

- `charges` — medical insurance cost

Url:
- https://www.kaggle.com/datasets/mirichoi0218/insurance

# What I did

In this project I worked with:

- Exploratory Data Analysis (EDA)
- Missing values checking
- Correlation analysis
- Categorical feature encoding
- One-Hot Encoding
- Feature scaling with StandardScaler
- Train/Test split
- Linear Regression
- ElasticNet Regression
- Model evaluation

# Preprocessing

Numerical features were scaled using `StandardScaler`.

Categorical features were converted into numerical features using `OneHotEncoder`.

I used `ColumnTransformer` to apply different preprocessing methods to different types of features.

# Models

I compared two models:

- Linear Regression
- ElasticNet

ElasticNet was used to check whether regularization could improve the performance of the basic Linear Regression model.

# Results

# Linear Regression

- MAE: ~$4,052
- RMSE: ~$5,956
- R² on test set: ~0.762

# ElasticNet

- MAE: ~$4,052
- RMSE: ~$5,956

The results of Linear Regression and ElasticNet were almost identical.

In this experiment, ElasticNet did not provide a meaningful improvement over Linear Regression, so the simpler Linear Regression model was a reasonable choice.

# What I learned

This project helped me practice working with categorical and numerical features in the same dataset.

I also learned how to use `ColumnTransformer`, `OneHotEncoder`, `StandardScaler`, and compare different regression models using MAE, RMSE, and R².

# Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab
- Jupyter Notebook
