# PROJECT TITLE:

-Analysis on Unemployment in the Context of COVID-19

# PROBLEM STATEMENT:

-The COVID-19 pandemic caused unprecedented economic disruptions worldwide, leading to job losses across multiple sectors. However, the impact was not uniform across countries, age groups, and genders. There is a need to systematically analyze unemployment trends before, during, and after COVID-19 to understand which populations were most affected and how recovery patterns differ globally.

# OBJECTIVES:

1. **Trend Analysis**-To analyze global unemployment trends from 2014 to 2024 and identify significant changes during the COVID-19 period.

2. **COVID Impact Assessment**-To quantify the impact of COVID-19 on unemployment by comparing pre-COVID (2014–2019), COVID (2020–2021), and post-COVID (2022–2024) periods.

3. **Demographic Analysis**-To examine how unemployment trends varied across different age groups and genders during the COVID-19 period.

4. **Country-Level Analysis**-To identify countries that experienced the highest increase in unemployment during COVID-19 and analyze their recovery patterns.

5. **Prediction & Forecasting**-To build predictive models that forecast unemployment trends based on historical data and evaluate post-COVID recovery patterns.

6. **Visualization & Accessibility**-To present insights through interactive visualizations and a web-based dashboard for easy interpretation by non-technical users.

# DATASET DESCRIPTION:

-**Dataset Name**-global_unemployment_data
-**Dataset Source**-https://www.kaggle.com/datasets/sazidthe1/global-unemployment-data
-**Column Number**-15
-**Row Number**-1135
-**Time Period Covered**-2014-2024
-**COVID-19 Timeline**-2020-2021
-**Pre-COVID**-2014-2019
-**Post-COVID**-2022-2024
-**Attributes Present:**
-country_name
-sex
-age_group
-age_categories
-**Age Categories:**
-Youth(15-25)
-Adult(25+)
-Children(under 15)

# PROJECT WORKFLOW:

1. Data Collection
2. Data Cleaning & Preparation
3. Exploratory Data Analysis (EDA)
4. Prediction Modeling

# KEY INSIGHTS:

1. **Global Yearly Trend:**
- Pre-COVID started high in 2014(due to the after-effects of 2007-2009 Great Recession) but was showing signs of decrease in unemployment before COVID.
- Global unemployment increased sharply during 2020 and 2021, indicating the significant economic impact of COVID-19.  
- Post-2021, unemployment levels shows a sudden drop of unemployment rates.

2. **COVID Phase Comparison:**
- Pre-COVID was initially high but was gradually decreasing until COVID.
- The COVID phase recorded the highest average unemployment rate, clearly indicating the economic disruption caused by the pandemic.  
- Post-COVID unemployment declined significantly better than Pre-COVID rates, showing sudden decrease in unemployment rates after COVID-19

3. **Age & Gender-wise Unemployment Analysis:**
- Adults experienced better recovery than Youth from unemployment
- Males experienced better recovery than Females from unemployment
- Indicates Youth Age categories always having higher unemployment rates than Adult Age categories
- Indicates Females experience more unemployment than Males

4. **Country-wise Unemployment Impact Analysis:**
- Most of the countries suffering from high unemployment come from Africa and West Asia
- Djibouti has the highest and Cambodia has the lowest unemployment rates during COVID phase
- In the top 5 highest unemployment rate countries, only South Africa didn't recover as its rates kept increasing even Post-COVID

5. **India's Unemployment Analysis:**
- India had a higher unemployment rate at 2018 due to slow job creation in manufacturing/industry, the disruptive impacts of demonetization (2016) and the GST rollout (2017) on small businesses, a growing skills gap between education and industry needs, and structural issues like agricultural distress
- However, India did make a recovery Post-COVID phase with 10.5% unemployment rate in 2024
- Difference between Male and Female in unemployment rates were consistent during Pre-COVID and COVID phases, but at Post-COVID, Females had a lesser unemployment rate than Males due to lesser Females participating in job hunts and more Females focusing on family labor which isn't captured in the census
- The Youth have a higher unemployment rate than the Adults as the Adults have better recovery throughout
- Youth unemployment is overall massive with over 20%, with Female Youth experiencing slightly less unemployment rates 
- Adult unemployment is better as its under 6%, with Female Adults experiencing under 5% unemployment rates

# PREDICTION/FORECASTING:

- Linear Regression (World Unemployment Rate)
- Features: Year, COVID Phase (encoded)
- Metrics: R², MAE
- Prediction accuracy is very poor due to the following facts:
1. The use of weak features such as year and COVID phase(Time doesn't cause unemployment)
2. Lack of more features such as economic indicators(GDP Growth, Inflation Rate, Interest Rates), month data, population, government policy, war, labor laws, etc.
3. Wrong Model usage, since Linear Regression fails to capture the outliers in a straight line(However, no model would provide accurate results without more features)
4. The presence of outliers as large as 80%(But these outliers are correct data and are needed to be presented in the predictions)
5. High heterogeneity by using all countries to predict world unemployment rate(Too many factors to calibrate for each country makes this an impossible to predict)

# TECHNOLOGY USED:

-Python(Jupyter Notebook)
-Python Libraries:
1. Numpy
2. Pandas
3. Seaborn
4. Matplotlib.pylot
5. Scikit-learn
-Excel(Power Query)

# AUTHOR:

### Name-Nithishvar M
### Degree-Bsc.Data Science

