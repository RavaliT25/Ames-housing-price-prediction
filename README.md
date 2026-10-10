# Ames Housing Data Analysis and Sale Price Prediction

## Project Overview

This project analyzes housing data from Ames, Iowa, to understand the factors associated with house sale prices and build a machine learning model to predict sale prices.

Using Python, NumPy, Pandas, Seaborn, Matplotlib, and Scikit-learn, the project covers data inspection, statistical analysis, data cleaning, exploratory data analysis, feature engineering, and Linear Regression.

## Objectives

- Explore housing prices and property characteristics.
- Analyze price differences across neighborhoods.
- Investigate the relationship between house quality, construction year, lot area, and sale price.
- Identify potential sale-price outliers.
- Build a Linear Regression model to predict house sale prices.
- Evaluate model performance using R², RMSE, and MAE.

## Dataset

The project uses an Ames Housing subset containing 2,930 house records.

Key features include:

- `SalePrice` — house sale price and prediction target.
- `Neighborhood` — location of the property.
- `Year Built` — original construction year.
- `Overall Qual` — overall material and finish quality.
- `Kitchen Qual` — kitchen quality rating.
- `Exter Qual` — exterior quality rating.
- `Lot Area` — lot size.
- `PID` — property identification number.

## Tools and Technologies

- Python
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## Project Workflow

### 1. Data Inspection
- Load and inspect the dataset.
- Check dataset dimensions, data types, missing values, and duplicate property IDs.

### 2. Statistical Analysis with NumPy
- Calculate mean, median, standard deviation, minimum, maximum, and quartiles of sale prices.
- Calculate sale price relative to lot area.
- Classify houses using the median sale price.
- Count houses built after 2000.
- Identify statistical outliers using Z-scores.

### 3. Data Cleaning and Exploration with Pandas
- Remove unnecessary columns.
- Explore neighborhood distributions and sale-price statistics.
- Calculate house age.
- Identify high-quality houses below a specified price threshold.
- Analyze kitchen and exterior quality ratings.

### 4. Data Visualization
- Compare average sale prices across neighborhoods.
- Visualize overall house quality ratings.
- Examine kitchen and exterior quality distributions.
- Analyze the number of houses built across decades.

### 5. Feature Engineering
- Create house-age and quality-score features.
- Group overall quality into descriptive categories.
- Explore a quality-to-price value score.

### 6. Machine Learning: Linear Regression
- Select relevant features for predicting `SalePrice`.
- Convert quality ratings into numerical scores.
- Apply one-hot encoding to neighborhood.
- Split the data into training and testing sets.
- Train a Linear Regression model using a Scikit-learn pipeline.
- Evaluate predictions and inspect model coefficients and residuals.
- Generate a sale-price prediction for a sample house.

## Model Performance

The Linear Regression model produced the following results on the test set:

| Evaluation Metric | Result |
|---|---:|
| R² Score | 0.779 |
| RMSE | $42,116.07 |
| MAE | $27,676.85 |

The model explains approximately 77.9% of the variation in test-set sale prices. The MAE indicates an average absolute prediction error of approximately $27,677.

## Key Skills Demonstrated

- Data cleaning and preprocessing
- Exploratory data analysis (EDA)
- Statistical analysis with NumPy
- Data manipulation with Pandas
- Data visualization
- Feature engineering
- Categorical encoding
- Linear Regression
- Model evaluation and interpretation
- Python functions and analytical problem-solving

## How to Run the Project

1. Clone or download this repository.
2. Install the required Python libraries.
3. Ensure the dataset is available at the path used in the notebook.
4. Open `ames housing v.03.ipynb` in Jupyter Notebook or JupyterLab.
5. Run the cells in order.

Install the main dependencies with:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

## Conclusion

This project combines exploratory data analysis with a supervised machine learning approach to investigate housing prices. It demonstrates a complete introductory analytics workflow, from examining raw data and engineering features to training, evaluating, and interpreting a regression model.

## Future Improvements

- Test additional regression algorithms.
- Explore more housing features.
- Tune model parameters and compare performance.
- Improve the analysis of prediction errors.
