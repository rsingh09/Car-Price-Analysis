# Used Car Price Analysis

### Summary of Findings

This analysis aimed to identify the factors that influence used car prices using a dataset from Kaggle. Key findings from the analysis are as follows:

1. **Car Age:** Older cars tend to have lower prices. The 'car_age' feature had a significant negative impact on car prices.
2. **Odometer Readings:** Higher mileage is associated with lower car prices. There is a clear negative correlation between odometer readings and car prices.
3. **Manufacturer:** Certain manufacturers, such as Ferrari, Land Rover, and Tesla, command higher prices, while others like Ford and Chevrolet have lower average prices.
4. **Model:** Specific models, such as the Land Cruiser HDJ81 - 80 series and Skyline GTR R32, significantly increase car prices.
5. **Condition:** Cars in 'excellent' and 'like new' condition fetch higher prices compared to those in 'good', 'fair', or 'salvage' condition.
6. **Fuel Type and Transmission:** Diesel and electric cars generally have higher prices compared to gas cars. Manual transmission vehicles tend to have slightly lower prices compared to automatic ones.
7. **Non-linear Relationships:** Polynomial features, particularly the cubic term for car age, showed a substantial impact on pricing, indicating non-linear relationships in the data.

The Ridge regression model, incorporating polynomial features and hyperparameter tuning, achieved a higher R-squared value of 0.6379, indicating better explanatory power compared to the simple linear regression model with an R-squared value of 0.5741.

### Recommendations
Based on these findings, the following recommendations are made for the used car dealership:
1. Focus on acquiring newer cars with lower mileage to attract higher prices.
2. Maintain a diverse inventory with popular high-value manufacturers and models.
3. Ensure that cars are in excellent or like-new condition to maximize their resale value.
4. Consider the benefits of offering diesel and electric vehicles, which are valued higher in the market.
5. Utilize advanced modeling techniques to capture non-linear relationships and better predict car prices.

## Link to Notebook
[Used Car Price Analysis Notebook](car-price-analysis.ipynb)

## Project Organization
The project is organized into the following sections:
1. **Data Understanding:** Initial exploration of the dataset to understand its structure and characteristics.
2. **Data Preparation:** Cleaning and transforming the data for analysis and modeling.
3. **Exploratory Data Analysis (EDA):** Visualizing the distribution of key variables and relationships between them.
4. **Modeling:** Building and evaluating regression models to identify factors influencing car prices.
5. **Future Analysis Recommendations:** Suggestions for further analysis to enhance insights.

## Usage Instructions
To use this notebook, follow these steps:
1. Install the required libraries: pandas, numpy, seaborn, matplotlib, plotly, sklearn.
2. Load the dataset `vehicles.csv` into the notebook.
3. Run the notebook cells in sequential order to reproduce the analysis.

## Directory and File Information
- **car-price-analysis.ipynb:** Jupyter notebook containing the full analysis.
- **vehicles.csv:** Dataset file used for the analysis.
- **images/**: Directory containing visualizations generated during the analysis.

## Additional Notes
- Assumptions: Missing values were handled using median imputation for numerical columns and mode imputation for categorical columns.
- Limitations: The analysis may not account for all factors influencing car prices. Further analysis is recommended to incorporate additional features and external economic indicators.
