# Linear and Polynomial Regression
## Program use linear and polynomial regression of second degree to predict progress in solving the rubik's cube 3x3 
### 1 Data preparation
CSV file includes number of solving the rubik's cube and solving time in seconds.
Solving time was transform from string type to float some data has incorrect values for example solving time in format: 25.April. 
**Function:** pd.to_numeric(data_df['solution_time_seconds'], errors='coerce') changed values to float type if values was incorrect solving time changed to null.
Next I used dropna to removed rows with null values.
# 2 Linear Regression
1. I used scikit-learn library to split data into training and testing set
2. Data standardization using StandardScaler
3. Model is trained and next is evaluate
4. Used matplotlib to draw a chart
# 3 Polynomial Regression Degree=2
1. Data are trained and transformed for polynomial regression
2. Model of linear regression use transformed data to make predictions
