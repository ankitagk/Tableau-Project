# Tableau-Project

Need for Workforce Development Plan for New York State Authority (NYSA)         
Collected, Collated & Cleaned 80+ data files from Bureau of Labor Statistics (BLS) across 7 different industries using Tableau Prep. 
Performed data modelling using CRISP-DM technique, created dashboards, identified 50% of working employees are located in NYC and forecasted 7 MM employee count in NYC by end of 2019; ow NYSA need to create job opportunities in other cities
. You can follow all the steps of CRISP-DM technique in detail below.

BUSINESS UNDERSTANDING
New York State Authority (NYSA) wants to create a workforce development plan to align with the needs and priorities of the state’s workforce and economic development objectives. To achieve this, NYSA is planning to analyze the past 10 years of performance on parameters such as hourly pay, inflation rate, hiring trend for the workforce and employee growth rate across various industries. 
Data for factors stated in the earlier paragraph would be required to build the analysis report. Bureau of Labor Statistics’ (BLS) Occupational Employment Statistics (OES) program produces employment and wage estimates for over 800 occupations. These are estimates of the number of jobs in certain occupations, and estimates of the wages paid to them. BLS’ comprehensive inventory will be used for our data analysis. 
For our analysis, we will use Tableau tools: Tableau Prep to combine data across 80+ worksheets, Tableau Desktop to model the data and Tableau Public to deploy the final version. Economic factors such as GDP, inflation will be affecting the employment growth rate and salaries; we assume that the data provided by BLS will help us determine the data quality. Additionally, missing values will be ignored from our calculations which might lead to deviations from the actuals.  Seasonally adjusted data evens out periodic swings in statistics; thus, to capture the actuals, non-seasonally adjusted has been used for our analysis.
The goal of our project is to assist NYSA in workforce planning by forecasting industry and labor force trends, correlate between minimum wage and employment growth rate, and concentration of employees across various industries.
 
DATA UNDERSTANDING
Bureau of Labor Statistics (BLS) provides data for the nation as a whole, for individual States, and for metropolitan statistical areas (MSAs), metropolitan divisions, and nonmetropolitan areas; national occupational estimates for specific industries are also available. On a high-level, we have categorized the data into 7 industries: construction, information, leisure, manufacturing, professional and business, transportation and utilities & other services.
To cater to the NYSA’s requirement, we will be creating reports to compare the number of employees, employment forecast, change in employment rate, hiring trend, inflation rate & wage details. We would be leveraging the data from 2008 to 2018 maintained by BLS. The number of employees: worksheets with details of the number of employees in NY state and NYC have been used. NYC, being the dream destination of working professionals across the globe, was chosen for comparison. The number for all industries is listed in 1000s(K). Wage Details: average hourly rates of the employees across industries are listed for a particular month of a year in terms of $ up to two decimals. Working hours: similar to hourly rates, average hours that a professional work for is available. Hourly rate & working hours can be used to compute the average annual salary. Inflation rate: the data reflects 12-months percent change. 
The data across all the 7 industries can be collated using Tableau Prep for comparison. The collation of data would significantly trim down 80+ files that we are referring to. Each of the new files will have columns for the industry, month and year; these columns can be used to compare attributes across different worksheets. Though there are few missing values, the overall data is good. We, for our analysis, will be ignoring all the null values which might impact the actual average values. However, the impact is not expected to be huge.
                                                           DATA PREPARATION

In our study, we have considered the number of employees, Average hourly rate, weekly working hours, yearly, monthly data for seven different categories of industries such as construction, information, leisure, manufacturing, professional and business, transportation and utilities & other services. Each industry category data can be classified in various industries but we have excluded the sub-category classification of data in our analysis. We have considered 10 years of data from 2008 to 2018. All the above data have been collected for both New York State and New York City. Last 10 years’ data of the inflation rate of the United States has also been used in our analysis. All the data is collected from the Bureau of Labor Statistics (BLS) repository. We have used around 88 worksheets in Tableau Prep for data cleaning, creating records, merging and aggregating the data mainly into 5 worksheets for our complete analysis.
 In Tableau Prep we uploaded the BLS Time Data series CSV file for each category and cleaned the source file by removing extra string messages. We initially had monthly data and we pivoted these values to get the yearly data and combined it with all the seven industries data. We have prepared “Employee” worksheet which contains the number of employee information by cleaning BLS Time Series Data, pivoting it based on the year and combining the data across the 7 different industries. We prepared the number of employee details for New York State and New York City. Similarly, we have also collated the weekly hours and hourly wage data separately by month, year and each industry. For the entire process flow diagram of combining data in Tableau Prep, kindly refer the below diagram. We can blend the data in tableau from different sources, giving an example we have blended the number of employee data for New York State and New York City. We have used various fields such as the number of employees, hourly rate, hourly wage to calculate aggregate values such as employee growth rate, average hourly rate, etc. 
Process Flow Diagram of Combining Data in Tableau Prep
  
MODELLING

To model our data and prepare our reports, Tableau tools have been used. Our design are as follows:

Industry Wise Number of Employees in NY state v/s NYC:
The report gives industry-wide distribution of the number of employees in New York state with those in New York City. For e.g.: in Information industry, 74% of NY state’s workforce is concentrated in New York city.
 

Annual % change in the number of employees in NY state:
The report shows decline in the number of employees in the 2009 and 2010, and steady growth in the following years. It also, shows an over-all positive trend.
 


Quarterly % change in number of employees across various industries:
It can be observed that most of the hiring happens in quarters Q2 & Q4, and we can see a drop in the number of employees in quarters Q1 & Q3 across all the industries. From the data, it can be inferred that Construction and Leisure are affected the most.
 
NYC Employee Forecast:
Based on the trend and the average growth, we have forecasted the number of employees in NYC till the year 2020. We expect a drop in 2019 Q1, and the number to rise to 7,046 k till end of 2019.
 
% Change in salary with respect to inflation:
This report compares the percentage change in salary with the inflation rate. The average percentage change in salary is correlated with the inflation rate, however, individual industries do not follow the same pattern. 
 
Weekly working hours and hourly wage for various industries:
 

Industry Rank with respect to Hourly pay:
The industries have been ranked based on the hourly wages through 2008 to 2017. It can be seen that “Information” industry has always topped the charts.
 
 
EVALUATION
Dashboard: 
-	It can be observed that within the state of New York more than 50% of working employees are located in New York City.

-	As per our analysis, the employee count is forecasted to cross 7 million in New York City by end of 2019.

-	So, the New York state government needs to develop workforce plan to create job opportunities in other cities of New York.

-	Also, the New York state government should make a note of and analyze the sudden percentage change in hiring across the quarters; Q1 shows fall & Q2 shows rise. 


 
 
 
DEPLOYMENT
The report can be viewed on Tableau Public using following links:
https://public.tableau.com/profile/ankita4666#!/vizhome/Final_15539731804730/NY-SalaryHours?publish=yes
https://public.tableau.com/profile/ankita4666#!/vizhome/Final_15539731804730/NY-Employees?publish=yes
