
## SALES FORECASTING USING TIME SERIES ANALYSIS


- This project aims to analyze historical sales data, clean and preprocess it, and apply time series forecasting techniques to generate accurate future predictions.
- Additionally, I have created a dashboard to visually present the insights, making the data more accessible and actionable.

# Objectives


- Preprocess and clean historical sales data.  
- Perform exploratory data analysis (EDA) to identify trends and seasonality.  
- Build a time series forecasting model.  
- Evaluate the model’s performance using statistical metrics.  
- Develop a Tableau dashboard for sales visualization.  
- Provide business insights and recommendations.  

# Tools & Technologies Used
Programming & Libraries:
- Python (Jupyter Notebook)  
- pandas, numpy: Data manipulation  
- matplotlib: Data visualization  
- statsmodels: Statistical analysis  
- Prophet: Time series forecasting  
- sklearn: Model evaluation  

# Visualization:
- Matplotlib for data visualization  
- Tableau for interactive dashboarding  


# Data Export:
- CSV files for cleaned and forecasted data  

# Data Preprocessing:
-To ensure data quality and accuracy, the following steps were taken:

1. Loading the Dataset:
   - The dataset was loaded from stores_sales_forecasting.csv.

2. Data Cleaning & Transformation:  
   - Selected relevant columns: Order Date and Sales.
   - Converted Order Date to datetime format for time series processing.
   - Set Order Date as the index.

3. Outlier Detection & Removal:
   - Applied the Interquartile Range (IQR) method to remove extreme sales values.

4. Resampling Data:
   - Aggregated sales data into monthly intervals to smooth fluctuations.

5. Feature Engineering:  
   - Created a lag feature (“Sales.L1”) to help in predictive modeling

# Exploratory Data Analysis (EDA) & Dashboard Insights
Key Findings 
- A box plot was used to detect and remove outliers.
- The Augmented Dickey-Fuller (ADF) test confirmed that the data required transformation for stationarity.

# VISUALIZATION
## Tableau Dashboard Analysis:


![Dashboard Preview](Visualization_Task_2.png)



## Comparison of Actual vs. Forecasted Sales (2017):
- Forecast Accuracy Trends
In some months (March, April, and December), forecasted sales closely align with actual sales, indicating the model performs well in stable periods.
- Underestimation & Overestimation Trends.	
Underestimation (Actual Sales Vs Forecasted Sales)
- June, November, December 2017 - Indicates that the model did not fully capture seasonal demand spikes or external factors.
Overestimation (Forecasted Sales > Actual Sales)
- March, May, August 2017 → Suggests that the model predicted higher sales than what was actually recorded, possibly due to incorrect seasonal trend assumptions.

##  Seasonality & Unexpected Spikes
- June 2017 saw the highest actual sales, indicating a potential seasonal trend or external event.
- Sales stabilized from August to October, where the forecast was more aligned, indicating better model performance in steady sales months.

Sales Trends Over Time: 
  - A line chart was used to visualize trends in both actual and forecasted sales.
  - The trend follows a predictable pattern with fluctuations due to seasonality.
