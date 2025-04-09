# project-hyperlaunch
# YouTube Earnings Prediction using Machine Learning

This project builds a machine learning model to **predict the average monthly earnings of YouTubers** using key metrics like subscribers and video views. It includes data preprocessing, correlation analysis, supervised regression modeling using **Random Forest**, and visual evaluation of model predictions.

----

## Objective

To develop a **data analysis application** using a supervised learning model to predict monthly YouTube earnings based on numerical metrics.

---
## Dataset

Name: Global YouTube Statistics.csvSource: [Kaggle / Public Dataset]
----


## Features include:

* Youtuber (Channel Name)

* Subscribers

* Video Views

* Likes

* Comments

* Category

* Lowest Monthly Earnings

* Highest Monthly Earnings

## Target Variable: Average Monthly Earnings (calculated)

----
## Project Workflow
1.  Data Loading
• Loaded dataset using pandas.

• Checked shape and structure of the data.

• Displayed key statistics using .info() and .describe().

2. Data Preprocessing
• Handled missing values:

• Categorical columns → filled with mode.

• Numerical columns → filled with mean.

• Checked for and removed duplicate rows.

• Created a new column:
   avg_monthly_earnings = (lowest + highest earnings) / 2

• Encoded categorical variables using LabelEncoder.

3. Exploratory Data Analysis (EDA)
∘ Visualized:

 ∘ Distribution of Average Monthly Earnings (Histogram)

 ∘ Channel Count by Category (Bar Chart)

 ∘ Correlation Heatmap between Subscribers, Views, and Earnings

4.  Model Building
∘ Model Used: RandomForestRegressor

 ∘ Split: 80% Training / 20% Testing

 ∘ Selected features: Subscribers, Views, Likes, Comments, etc.

5.  Model Evaluation
∘ Evaluation Metrics:

 ∘ R² Score: 0.995 → Excellent accuracy

 ∘ RMSE: ~₹36,897

 ∘ MAE: ~₹7,800

 ∘ These metrics show the model performs with high precision and low error.

6.  Visualization & Results
 ∘ Scatter Plot: Actual vs Predicted Earnings → Most dots near diagonal = accurate predictions.

 ∘ Residual Plot: Distribution of prediction errors → Centered and minimal.

 ∘ Bar Plot: Top 10 YouTubers → Visual comparison between actual and predicted earnings.
----
## Key Insights
 ▪ Channels with high Subscribers and Views tend to have higher earnings.

 ▪ Random Forest Regression handled non-linear relationships and noise effectively.

 ▪ Model can generalize well on unseen data.
---
## How to Use
 ▪ Requirements
    ▪ Install these Python packages before running:

 ## bash

pip install pandas numpy matplotlib seaborn scikit-learn
----
## Steps to Run
  ▸ Download the dataset: Global YouTube Statistics.csv

  ▸ Run the notebook: YouTube_Earnings_Prediction.ipynb

##  Follow the workflow cells to:

 ▸ Load & clean data

 ▸ Train the model

 ▸ Evaluate results

 ▸ Visualize insights
-----

## Conclusion
  ● Built a reliable earnings prediction model for YouTube creators.

  ● Gained insights into how channel stats affect earnings.
 
  ● Used Random Forest Regressor for robust performance.

  ● Delivered meaningful visualizations and accurate estimates.

-------
## Future Improvements
   ● Add a web interface for real-time predictions using Streamlit or Flask.

   ● Incorporate more data like engagement rate, watch time, country, etc.

   ● Experiment with other models like XGBoost or Neural Networks.
----
