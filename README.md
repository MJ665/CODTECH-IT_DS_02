
---

# Linear Regression Model for California Housing Dataset

## Overview
This project demonstrates how to build a simple Linear Regression model using the California Housing dataset to predict the median house value based on features like median income, average rooms, average occupancy, and house age.

The workflow includes:
- Loading and exploring the dataset.
- Preprocessing and splitting the data into training and test sets.
- Training a Linear Regression model.
- Evaluating the model's performance using metrics such as Mean Squared Error (MSE) and R-squared (R²).
- Visualizing the model's predictions versus actual values.
- Providing a CLI for users to input new data and make predictions.

## Requirements
- Python 3.x
- pandas
- numpy
- matplotlib
- scikit-learn

You can install the required libraries using pip:

```bash
pip install pandas numpy matplotlib scikit-learn
```

## Dataset
This project uses the **California Housing dataset** from the `sklearn.datasets` module, which includes data on housing prices in California. The dataset contains information about:
- `MedInc`: Median income in block groups.
- `AveRooms`: Average number of rooms per household.
- `AveOccup`: Average number of occupants per household.
- `HouseAge`: Median age of houses within a block.
- `MedHouseVal`: Median house value for California's districts, the target variable.

## Steps in the Code

### 1. Load and Explore the Dataset
The dataset is loaded using the `fetch_california_housing` function from `sklearn.datasets`. The features `MedInc`, `AveRooms`, `AveOccup`, and `HouseAge` are selected to predict the target variable `MedHouseVal`.

### 2. Data Preprocessing
The dataset is split into training and testing sets using `train_test_split` from `sklearn.model_selection`.

### 3. Train the Linear Regression Model
A Linear Regression model is trained using the selected features and target variables. The model is then used to predict the median house values for the test set.

### 4. Model Evaluation
The model's performance is evaluated using:
- **Mean Squared Error (MSE)**: Measures the average of the squares of errors.
- **R-squared (R²)**: Measures the proportion of variance in the dependent variable explained by the model.

### 5. Visualizing Predictions
A scatter plot is created to visualize the actual vs. predicted values, with an ideal fit line shown in red.

### 6. Prediction CLI
A command-line interface (CLI) allows users to input new values for `MedInc`, `AveRooms`, `AveOccup`, and `HouseAge` to predict the median house value. The user can input values as comma-separated values, and the model will output the predicted value.

### Example Prediction
- **Example Input**: `3.5, 6.0, 3.0, 20`
- **Output**: Predicted median house value based on input features.

## Results
- **Model Performance**:
  - **Mean Squared Error (MSE)**: `Value`
  - **R-squared (R²)**: `Value`
- Visualizations will display the accuracy of the predictions in comparison to the actual test data.

## Conclusion
This project demonstrates how to use a linear regression model for predicting continuous target values, with an interactive CLI for real-time predictions. The performance of the model can be improved by exploring additional features or using more advanced techniques.

---

