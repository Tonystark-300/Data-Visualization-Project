# Data-Visualization-Project
semester  V project - Data Management ans Analysis
The following project is about analysis of IPL dataset from 2008 to 2019 year. 
Dataset used in the following Visualization has been taken from kaggle.com .Kaggle is the world's largest data science community with powerful tools and resources to help you achieve your data science goals. Kaggle allows users to find and publish data sets, explore and build models in a web-based data-science environment, work with other data scientists and machine learning engineers, and enter competitions to solve data science challenges.
link of dataset: https://www.kaggle.com/ramjidoolla/ipl-data-set

Tool used : Ms Excel, Tableau prep builder. 
Various visualization techniques have been used like
 - charts 
 - pivot table 
 - data models, etc.

**Introduction:**

Data analysis is important in business to understand problems facing an organization, and to explore data in meaningful ways. Data in itself is merely facts and figures. To know how to analyze data is an important skill to learn nowadays. It answers many questions that tends to get raise in future. So, it is a big help to know the answers already and for that data should be analyzed thoroughly. This project is meant to be a good practice of doing data analysis.

The dataset on which I worked, consists of data about IPL matches played from the year 2008 to 2019. IPL is a professional Twenty-Twenty cricket league founded by the Board of Control for Cricket in India (BCCI) in 2008. The league has 8 teams representing 8 different Indian cities or states. It enjoys tremendous popularity and the brand value of the IPL in 2019 was estimated to be ₹475 billion (US$6.7 billion).                                               


**Objectives of the analysis**

1.	To show number of matches won by every team season wise.
2.	To find top 10 batsman.
3.	To find the player with most man of the match award.
4.	To find the venue that hosted maximum number of IPL matches.
5.	To find whether winning a toss increases the chances of victory.
6.	Find country to which batsman with highest score belongs.
7.	Country wise analysis of left-hand and right-hand batsman.

**Dashboard :**
![dashboard](https://user-images.githubusercontent.com/61225994/107218346-81e4d280-6a35-11eb-9b17-69fa7d1a6e84.png)


#**ETL Process**<h1>
Cleaning of matches.csv file:
Removal of NULL values-
There are 756 rows and 18 columns in matches.csv file. 756 rows imply that there were 756 IPL matches held between 2008- 2019.
![process1](https://user-images.githubusercontent.com/61225994/107217787-b1dfa600-6a34-11eb-876a-5cab2189741a.png)

Data indicates the presence of 637 Null values in Umpire3 column. It’s of no use of knowing about the count of null values. This column has a significant number of Null values in compare to others so, remove umpire3 column.
Removal of those columns which are not needed-
Umpire1 and Umpire2 are not needed in my data analysis. So, remove those columns.
Keep fields: [id, Season, city, team1, team2, toss_winner, player_of_match, venue]
Cleaning of deliveries.csv file:
Removal of NULL values-
There are 79K rows and 21 columns in deliveries.csv file. Out of which 1,70,244(95% rows) in player_dismissed column, 1,70,244(95% rows) in dismissial_kind and 1,72,630(96% rows) in fielder columns are NULL. So, remove columns  player_dismissed, dismissial_kind and fielder.

![process2](https://user-images.githubusercontent.com/61225994/107218022-0daa2f00-6a35-11eb-93b5-a7d45ccf5f1c.png)

Keep fields: [ match_id, batting_team, bowling_team, batsman, batsman_runs, total_runs]


**bold Word file for Reference and complete process.**
[end term report.docx](https://github.com/Tonystark-300/Data-Visualization-Project/files/5943680/end.term.report.docx)


