# KickStarter-Project

KickStarter Project

dataset source:https://www.kaggle.com/datasets/kemical/kickstarter-projects

Project Overview: This project delves into a comprehensive analysis of Kickstarter project data, focusing on project categories, years, countries, and pledged amounts in USD. By employing exploratory data analysis (EDA), data visualization techniques, and statistical analysis, our objective is to unearth valuable insights regarding the dynamics of popular categories across different countries and years, as well as identifying which categories garner the most pledges.

Dataset Description:

• ID: Unique identifier for each project order. • Name: Title of the project. • Category: Specific category of the project. • Main Category: Primary category classification of the project. • Currency: Currency corresponding to the project's country. • Deadline: Date by which the pledge goal must be reached. • Goal: Pledged monetary target. • Launched: Date of project launch. • Pledged: Total amount of money pledged. • State: Current status of the pledge. • Backers: Number of individuals who pledged money to the project. • Country: Country of origin for the project. • USD Pledged: Pledged amount converted to USD.

Analysis:

Loading Data: Import the dataset from a CSV file into a Pandas DataFrame.
Data Cleaning: • Check data types using the info() method. • Drop three columns with missing data. • Use dropna() to eliminate rows with missing values.
Determining the Most Popular Category: • Count the number of projects in each category. • Extract the top 5 most popular categories. • Visualize the top 5 categories using a chart for clarity.
Evolution of Primary Categories Over Years: • Convert the 'launched' column to datetime format, using errors='coerce' to handle any errors. • Extract the 'year' from the 'launched' column. • Filter data for years between 2009 and 2015. • Count the number of projects for each main category per year. • Identify the top 5 categories with the highest number of projects per year. • Visualize the evolution of category dominance over the years through a chart.
Top 5 Most Prevalent Categories for Each Country: • Identify the top 5 countries with the most projects. • Filter the data to include only these top 5 countries. • Group the data by 'country' and 'category' to count occurrences. • Determine the top 5 popular categories for each country. • Present the findings in a chart, highlighting the prevalence of each category in the top 5 countries.
Assessing Pledged Funds State within Each Category: • Identify the top 5 categories with the largest dataset. • Filter the dataset to include only these 5 main categories. • Determine the top 3 states with the largest dataset within each category. • Group the data by 'main_category' and 'state', counting occurrences. • Calculate the ratio of each category within each state. • Analyze the findings to understand the distribution of pledged funds states across categories.
Determining the Category with the Highest Goal among the Top 5: • Convert the 'goal' column to numeric type. • Calculate the average goal for each of the top 5 categories. • Identify the category with the highest average goal.
Identifying the Main Category with the Highest Amount of USD Pledges: • Convert the 'usd pledged' column to numeric type. • Group the data by main category based on the amount of USD pledged. • Determine the main category that received the highest percentage of USD pledges.
Examining Fluctuations in Pledge Amounts for Each Category Over Time: • Filter the dataset for the years 2009 to 2015. • Group the data by 'year' and 'main category'. • Analyze the trends in pledge amounts for each category over the specified time period.
Identifying the Category with the Most Significant Increase in USD Pledges from 2010 to 2015: • Compare USD pledged amounts between 2010 and 2015. • Determine which category experienced the largest increase in pledged funds during this period. • Interpret the findings to understand the growth dynamics across categories over time.
Conclusion:

After analyzing the dataset, it's evident that the most popular categories on Kickstarter are as follows: Film & Video, Music, Publishing, Games, Technology These figures highlight the enduring popularity of Film & Video projects, which consistently maintain the highest number of projects across the years. Additionally, there's a notable surge in Technology projects, particularly in 2014 and 2015, indicating a growing interest in this category. Conversely, Music projects have experienced a decline in attention since 2012. Publishing projects, on the other hand, exhibit steady growth over the analyzed period. Geographic Distribution of Projects:

The analysis reveals that the USA hosts a significantly higher number of projects compared to other countries.
The most popular categories in the USA include Project Design, Documentary, Music, Shorts, and Food. Success Rates Across Categories:
Music projects exhibit the highest success rate, followed closely by Film & Video.
However, Film & Video projects also have the highest number of canceled and failed states, indicating variability in project outcomes within this category. Goal Amounts by Category:
Technology projects set the highest goals, followed by Film & Video, Games, Publishing, and Music categories. Ease of Pledgement:
Games, Design, and Technology emerge as the categories with the highest percentages of successfully pledged funds, indicating greater ease of garnering pledges within these categories.
Music and Film & Video categories also show notable success rates in terms of pledged funds. Pledge Amount Trends Over Time:
Technology projects experienced a substantial increase in pledged funds each year, peaking in 2015.
Games projects have maintained relatively steady pledge amounts since 2012.
Film & Video projects reached their highest pledge amounts in 2013, with a gradual decline thereafter. Improvement in Pledged Funds from 2010 to 2015:
Games and Technology categories exhibit the most significant improvement in pledged funds over the five-year period.
Music, Theater, Dance, and Film & Video categories show comparatively smaller improvements in pledged funds during the same period.
In conclusion, this project provides valuable insights into the most popular Kickstarter categories, taking into account factors such as country and year. Through thorough data analysis using Pandas, we uncovered trends, patterns, and areas for improvement within the platform. By understanding the dynamics of project categories over time and across different regions, stakeholders can make informed decisions to enhance project success and drive business growth. The utilization of data analysis techniques allows us to extract actionable insights that can shape strategies and optimize outcomes within the Kickstarter ecosystem.
