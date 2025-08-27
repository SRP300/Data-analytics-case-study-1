The Global AI Landscape: An Investment Analysis of Industry Adoption and Economic Impact

# Scenario
Your manager has given you your first project to lead from start to finish.
Your new client is a venture capital firm preparing to launch a multi-million dollar fund dedicated to investments in the Artificial Intelligence sector. They need a data-driven report to ground their investment thesis in solid market evidence.You have been tasked with leading the entire engagement. This began with defining the business task: to conduct a comprehensive analysis of the global AI landscape to identify high-growth opportunities and provide actionable recommendations for capital allocation. You formulated the core strategic questions, focusing on the relationship between AI adoption and revenue, the impact of government regulation, and trends over time.
  

##  Description of Data Source
The foundation of this analysis is the Global AI Content Impact Dataset, a comprehensive collection of metrics detailing the influence of Artificial Intelligence across multiple sectors and nations. This dataset covers the period from 2020 to 2025, encompassing 10 distinct industries within 10 countries.   

A brief data dictionary for the key analytical columns is as follows:

AI Adoption Rate (%): The percentage of companies within a given sector that have integrated AI technologies into their core operations.

Revenue Increase Due to AI (%): The average percentage increase in revenue attributed directly to the implementation of AI solutions.

Top AI Tools Used: The most prevalent AI software or platform utilized within that market segment.

Regulation Status: The classification of the governmental regulatory environment concerning AI (Strict, Moderate, or Lenient).

Consumer Trust in AI (%): A measure of public confidence in AI technologies within a specific country.

In assessing the data's integrity according to the ROCCC framework (Reliable, Original, Comprehensive, Current, Cited), the dataset is evaluated as highly comprehensive, covering a wide array of metrics, geographies, and industries. Its currency, with data extending to 2025, allows for forward-looking analysis. For the purposes of this case study, the data is assumed to be reliable. This structured and complete nature of the data provides a strong foundation for the subsequent analysis. 

# Cleaning and Preparing Data for Analysis
A thorough and transparent data preparation process is essential to ensure the validity of any analytical findings. This section documents the tools and methodologies used to process the raw data and prepare it for strategic analysis.

## Tools for Transformation
The technical toolkit for this project was selected to reflect industry best practices and demonstrate versatility. Data cleaning and initial exploration were performed using R (leveraging the tidyverse suite) and SQL. The core analysis was conducted using SQL for data aggregation, while visualizations were generated using both Python (with matplotlib and seaborn) and R (with ggplot2).

## Documentation of Data Cleaning and Manipulation
Upon initial inspection, the dataset was found to be of high quality, with no missing values or significant data type inconsistencies. The primary data processing task was to standardize the column names, which contained spaces and special characters (e.g.,    

Revenue Increase Due to AI (%)). This format is incompatible with efficient querying in SQL and can be cumbersome in other analytical environments.

To address this, two methods were employed:

In R, the clean_names() function from the janitor package was used to programmatically convert all column headers to a consistent, snake_case format.

In SQL, a new table was created using a CREATE OR REPLACE TABLE statement, explicitly renaming each column to remove spaces and special characters (e.g., renaming AI Adoption Rate _%_ to AI_Adoption_rate).

This crucial, albeit simple, cleaning step ensures that the data is interoperable and ready for efficient analysis across multiple platforms. The high quality of the initial data allowed analytical resources to be shifted from time-consuming data cleaning to higher-value activities like modeling and deep analysis, thereby accelerating the path from data to decision-making.

# Guidelines to use code
Download dataset: https://www.kaggle.com/datasets/atharvasoundankar/impact-of-ai-on-digital-media-2020-2025?resource=download 
or from [clicking here](Data-analytics-case-study-1/Global_AI_Content_Impact_Dataset.csv)

1. Open [SQL queries](Data-analytics-case-study-1/SQL_queries) in preferred relational database
2. Open visuals made with [R code](Data-analytics-case-study-1/R_code) in preferred Integrated Development Environment or R terminal
3. Open [Python code](Data-analytics-case-study-1/Python_code) in preferred environment 

# Guiding Questions 

What is the relationship between the AI Adoption Rate and the Revenue Increase Due to AI across different industries?

Which industries have been the most aggressive in adopting AI-generated content over the last few years? 

Which industries is AI causing the most job displacement, and where is it creating successful human-AI collaboration?

Is there a positive correlation between adopting AI and increasing revenue or market share?

# Conclusion 
The analysis has yielded several key insights into the global AI landscape. First, there is a clear positive relationship between AI adoption and revenue, but the most significant growth potential lies in "Emerging" industries like Manufacturing and Media, where high ROI has been proven but market penetration remains low. Second, the ideal regulatory environment is nuanced; moderate regulation fosters the strongest commercial ecosystems, while lenient regulation correlates with higher public trust. Third, leadership in AI adoption, both nationally and industrially, is strongly linked to higher rates of job displacement, highlighting a critical socio-economic challenge. Finally, the impact of AI is not linear but cyclical, with significant fluctuations in adoption, revenue, and job loss over time.

Acess Analysis [powerpoint here.](Data-analytics-case-study-1/Data_analytics_project.pptx)
