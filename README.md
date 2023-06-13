Welcome to the documentation of the performance analysis of Titan FPL managers performance 2022/23. A personal project that combines my soccer hobby and analytics. The following steps were taken to document and make the project easily reproducible.

- Introduction:
 The 2022/23 season of Fantasy Premier League (FPL) was a record-breaking one, with over 11.4 million players competing for the top prize. 
Representing a 25% increase from the previous season. Titan FPL mini-league was Intensely contested among friends and colleagues, this could can be attributed 
to a number of factors, including the growing popularity of the game, the introduction of new features, and the increased prize money. This project will analyze
the performance of Titan FPL managers during the 2022/23 season. The analysis will focus on the following areas:

Team selection: How did Titan FPL managers select their teams? What factors did they consider when making their decisions?

Transfer strategy: How did Titan FPL managers manage their transfers? Did extra transfers really pay off? Did they take advantage of price rises and falls?

Overall performance: How did Titan FPL managers perform overall? How many managers finished in the top 100,000?

Objective: To identify the factors that contributed to Titan FPL's success in the 2022/23 season and provide insights into how other FPL managers can improve 
their own performance. The analysis will be conducted using various analytical tools such R, Excel and Power BI. The analysis will be presented in a clear and 
concise manner, and will be accompanied by visualizations to help illustrate the findings.

- Data Sources: The analysis will be conducted using a variety of data sources, including the official FPL website, the Fantasy Football hub website, and the Understat website. 

- Data cleaning: After collecting the titan fpl managers dataset, the first phase of the data cleaning was done in Rstudio. Using the head function, i viewed the top 5 rows of the dataset, also confiming the column names.
Using the dplyr and janitor packages, I removed the unwanted "#" column from the merged titan dataset. I also removed the "GW" prefix from the values in the game week column, converting it to a numeric datatype. Using the str function, i viewed
the internal structure of the dataset, making sure accurate data types were used for the different columns, the number of columns and rows are displayed. I also cleaned the column names and standardized them. After importing the file into power bi,
in the query editor, I promoted the headers, I also renamed the various columns. In the game week point difference column, I used Replace value changing NA to 0.

- Data transformation: The data will have to be transformed before it can be used. This involved changing the format of the data and converting it into a format that can be used by Power BI.

- Data Modeling: The first part of the data modeling was done using R in RStudio. Columns such as experience, favorite club, location, and game week points difference were created.
The second part of the data modeling was done in Microsoft Power BI. I used calculated columns to add new information to the data model, such as the total points for managers. I used
measures to create new metrics, such as the position of each manager at the end of Game week 38. This involved creating a data model that represented the relationships found between the different data sets. Some of the trends and patterns found in the data set included; the relationsship between overall rank 
and average squad value, managers with higher average squad values had better peformance, this could be due to their trasnfer strategy. There was no concrete relationship established between years of experience and overall performance, the manager mezzy_united
with about 6 years of experience came 26th out of 27. These data modeling techniques allowed me to create a powerful and flexible data model that could be used to analyze the performance of Titan FPL managers.

- Visualizations: Here are some of the key visualizations and insights presented in the report

- Overall Rank: This visualization shows the overall ranks of all the managers in the mini-league. The visualization shows that mavi_fc, whales_fc and premium_fc were the top 3 performing
managers in the Titan FPL mini-league 2022/23. This suggests that many factors were responsible for the various degrees of successes recorded.

- League Position: This visualization shows the position of managers in the league table. This can used to track the progress of managers over time, and to identify managers that are performing well or poorly.

- Years of Experience: This visualization shows the number of years of experience that players have. This type of visualization can be used to identify managers who are new to the game and managers who have been playing for a long time.

- Highest Rank Achieved: This visualization shows the highest rank that a manager achieved in a particular game week in the league or competition. The highest rank achieved will vary depending on their performance.

- Average Squad Value: This visualization shows the average value of squads of managers in the mini-league or competition. This type of visualization can be used to identify managers with teams that have a strong squad and teams that have a weak squad.

- Deployment: The deployment step is important because it makes the project available to users. This can be done by publishing the project to a Power BI service or by sharing the project with users.

- Limitations: In the course of this analysis, collecting data such as age, gender, and location were some of the data quality issues encountered. In future analysis, surveys, interviews and observations will be employed.

- Dependencies: This project does not rely on external libraries, APIs, or tools.

- Usage: Click on any of the managers to view their analytics. The visualizations are intereactive and responsive making navigating through the report/dashboard easy. 

- Maintenance and Updates: For the new FPL season 2023/24, I hope to create weekly and monthly perfomance anlaysis report/dashboards.
- Link to power bi project: https://app.powerbi.com/links/Iz0P9kIqTl?ctid=ae9af32b-72fc-4185-95bb-11103f434ac9&pbi_source=linkShare
