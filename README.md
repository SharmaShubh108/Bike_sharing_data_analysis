# **Demand for Electric Bicycles Analysis**

## **Project Overview**
This project analyzes the factors influencing the demand for Yulu's shared electric bicycles in the Indian market. Yulu, India’s leading micro-mobility service provider, has experienced revenue dips and seeks to identify key drivers of demand to optimize operations and boost revenue.

The project uses statistical analysis, visualizations, and machine learning to uncover trends, relationships, and insights within the provided dataset.

---

## **Problem Statement**
Yulu wants to address the following questions:  
1. Which variables are significant in predicting the demand for shared electric bicycles?  
2. How well do these variables describe the demand for electric bicycles?

---

## **Dataset**
The dataset (`bike_sharing.csv`) contains hourly aggregated data on bike usage with the following columns:

| **Feature**     | **Description**                                                                 |
|------------------|-------------------------------------------------------------------------------|
| `datetime`      | Hourly timestamp of the data                                                  |
| `season`        | Season of the year (1: Spring, 2: Summer, 3: Fall, 4: Winter)                 |
| `holiday`       | Whether the day is a holiday (1: Yes, 0: No)                                  |
| `workingday`    | Whether it is a working day (1: Yes, 0: No)                                   |
| `weather`       | Weather conditions (1: Clear, 4: Severe weather conditions)                   |
| `temp`          | Air temperature in degrees Celsius                                            |
| `atemp`         | Perceived ("feels like") temperature in degrees Celsius                       |
| `humidity`      | Air humidity in percentage                                                    |
| `windspeed`     | Wind speed in km/h                                                            |
| `casual`        | Number of bikes rented by casual users                                        |
| `registered`    | Number of bikes rented by registered users                                    |
| `count`         | Total number of bikes rented (casual + registered)                            |

---

## **Tools and Libraries**
- **Programming Language**: Python  
- **Libraries**:  
  - **Data Analysis**: `pandas`, `numpy`  
  - **Data Visualization**: `matplotlib`, `seaborn`  
  - **Statistical Analysis**: `scipy`  
  - **Modeling**: `scikit-learn`  

---

## **Project Steps**

1. **Data Loading and Exploration**  
   - Load and clean the dataset.
   - Perform exploratory data analysis (EDA) to understand trends and relationships.

2. **Feature Engineering**  
   - Extract time-based features (e.g., hour, day of the week, month) from the `datetime` column.  
   - Encode categorical variables (e.g., `season`, `weather`) using one-hot encoding.

3. **Exploratory Data Analysis (EDA)**  
   - Analyze demand across hours, days, seasons, and weather conditions.  
   - Visualize patterns and distributions to identify correlations.

4. **Statistical Analysis**  
   - Use **ANOVA** and correlation tests to determine significant factors impacting demand.  
   - Assess how weather, season, and other factors influence rentals.

5. **Modeling and Prediction**  
   - Build baseline models such as Linear Regression and more robust models like Random Forest.  
   - Evaluate model performance using metrics like RMSE and R².

6. **Insights and Recommendations**  
   - Derive actionable insights to improve bike utilization, optimize operations, and boost revenue.

---

## **Key Insights**
1. **Time-Based Trends**:  
   - Peak demand occurs during commute hours (8 AM and 6 PM).  
   - Weekends see higher rentals from casual users, while registered users dominate weekdays.

2. **Weather Impact**:  
   - Clear weather drives the highest demand.  
   - Severe weather (e.g., rain or snow) significantly reduces bike rentals.

3. **Seasonality**:  
   - Summer and fall exhibit the highest demand, while winter shows a noticeable dip.

4. **User Segmentation**:  
   - Registered users primarily rent for commuting, while casual users rent for recreational purposes.

---

## **Recommendations**
1. **Dynamic Fleet Allocation**:  
   - Increase bike availability during peak commute hours and weekends in high-demand zones.

2. **Dynamic Pricing**:  
   - Implement higher rates during peak hours and offer discounts during off-peak times or mild weather conditions.

3. **Subscription Plans**:  
   - Introduce flexible plans for registered users (e.g., monthly/annual passes) and bundled deals for casual users.

4. **Weather-Responsive Strategies**:  
   - Offer promotions or discounts during mild rain to improve rentals.

5. **Corporate Partnerships**:  
   - Collaborate with offices and universities to provide employee and student commuter plans.

---

## **Visualizations**
The project includes the following key visualizations:
1. **Hourly Demand Trends**: Bar plots of rentals across hours for casual vs. registered users.  
2. **Weather Impact**: Boxplots showing rental distribution across weather categories.  
3. **Seasonal Trends**: Visualizations highlighting differences in demand across seasons.  
4. **Feature Correlations**: Heatmaps showing relationships between demand (`count`) and features.

---

