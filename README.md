# Formula-1-Performance-Data-Analysis-

This project analysed a historical Formula 1 relational database (formula_1_2025_complete) containing data on drivers, constructors, races, circuits, race results, lap times and race statuses across multiple decades. The dataset was chosen because it provides a large, interconnected source of real-world sports data that is well suited to relational database analysis.

The aim of the project was to use SQL (MySQL) and Excel to explore historical Formula 1 performance and identify trends in driver success, constructor dominance, race calendar evolution, and circuit characteristics. The analysis addressed questions such as which constructors have historically dominated the sport, which drivers consistently achieved high performance, how Formula 1 seasons have expanded over time and whether certain circuit characteristics, such as altitude, may influence racing. By answering these questions, the project demonstrated how data analysis can be used to support performance evaluation, identify long-term trends and communicate insights through data visualisation and reporting.


---

## Table of Contents

- [Overview](#overview)  
- [Dataset](#dataset)  
- [Technologies Used](#technologies-used)  
- [Installation](#installation)  
- [Usage](#usage)  
- [Analysis & Visualizations](#analysis--visualizations)  
- [Conclusion](#conclusion)  
- [Credits](#credits)  
- [License](#license)  

---

## Overview

- **Motivation:**
I chose the historical Formula 1 dataset because it contains a rich collection of interconnected data covering drivers, constructors, races, circuits and race results over multiple decades. The dataset provided an opportunity to apply SQL to a realistic relational database while exploring a subject of interest. It also allowed me to develop practical skills in querying large datasets, identifying trends and communicating analytical findings through data visualisation.

- **Objective:**
The objective of this project was to analyse historical Formula 1 data to uncover patterns in driver performance, constructor success, race calendar evolution and circuit characteristics. The analysis aimed to answer questions such as:

Which constructors have historically dominated Formula 1?
Which drivers have consistently achieved strong career performance?
How has the number of races per season changed over time?
Which circuits have distinctive characteristics that may influence race performance?

The project also demonstrated how SQL and Excel can be used together to transform raw relational data into meaningful insights. 

- **Learning Outcomes:**
Working on this project strengthened my understanding of relational database analysis and the practical use of SQL for data analytics. I gained experience writing complex SQL queries using JOINs, aggregate functions, CASE statements and subqueries to analyse relationships across multiple tables. I also improved my skills in data cleaning, validation, exploratory data analysis (EDA) and presenting findings using Excel summary tables and charts. Overall, the project enhanced my ability to interpret large datasets, solve analytical problems and communicate data-driven insights effectively.

---

## Dataset

Provide details about the dataset used:

- Source of the Dataset:
The project used the formula_1_2025_complete historical Formula 1 database, which contains race data spanning multiple decades. The dataset includes information on drivers, constructors, races, circuits, race results, lap times and race statuses organised across multiple relational tables.

- Size of the Dataset (# of rows and columns):
The database consists of multiple relational tables containing tens of thousands of records. The largest tables store historical race results and lap times, while smaller tables contain reference information such as drivers, constructors, circuits and race statuses. Together, these tables provide a comprehensive dataset for analysing Formula 1 performance over time.

  
- Key Features/Columns Used:
The analysis focused on several core tables and their key attributes:

Drivers: Driver ID, name, nationality, date of birth.
Constructors: Constructor ID, team name, nationality.
Races: Race ID, year, race name, circuit ID, date.
Circuits: Circuit ID, circuit name, country, location, altitude.
Results: Driver ID, constructor ID, finishing position, points, race status.
Lap Times: Driver ID, lap number, lap time.
Race Statuses: Status ID and race outcome descriptions (e.g., Finished, Accident, Engine Failure).

These tables were linked using primary and foreign keys to perform relational analysis across drivers, teams, races and circuits.

- Data Preprocessing and Cleaning

Before analysis, the dataset was cleaned and validated to improve data quality and ensure accurate results. The preprocessing steps included:

Validating primary and foreign key relationships between tables.
Checking for missing values in critical fields.
Removing duplicate records where necessary.
Standardising country names and nationalities for consistency.
Verifying that numeric fields, including points, lap times and circuit altitude, were correctly formatted.
Performing validation checks in SQL and Excel to confirm the accuracy of summary statistics before conducting the analysis.

---

<h2>Technologies Used</h2>

<ul>
  <li><strong>Tools:</strong> Excel, Pivot Tables, SQL, Power Query, Conditional Formatting, VS Code, Git, GitHub</li>
</ul>

<p>
  <img src="https://img.shields.io/badge/Excel-3776AB?style=for-the-badge&logo=excel&logoColor=white" alt="Excel">
  <img src="https://img.shields.io/badge/Pivot_Table-150458?style=for-the-badge&logo=pivot_table&logoColor=white" alt="Pivot Table">
  <img src="https://img.shields.io/badge/Power_Query-013243?style=for-the-badge&logo=powerquery&logoColor=white" alt="Power Query">
  <img src="https://img.shields.io/badge/SQL-11557C?style=for-the-badge&logo=sql&logoColor=white" alt="SQL">
  <img src="https://img.shields.io/badge/Conditional_Formatting-4C72B0?style=for-the-badge&logo=conditionalformatting&logoColor=white" alt="Conditional Formatting">
</p>


---

## Usage

Instructions for using the project:

1. Open the main notebook (`analysis.ipynb`)  
2. Run each cell sequentially to reproduce the analysis  
3. Visualizations and results will be generated automatically  

Visualisations:

1. How many races were held in each decade?
Objective: Count the total number of races grouped by decade.


<img width="500" height="464" alt="image" src="https://github.com/user-attachments/assets/a25ed567-4c2c-4d61-b5c6-df816c51a7c7" />

2. Identify F1 Powerhouses – Constructors with 100+ Wins
Objective: Find constructors with more than 100 race wins.


<img width="550" height="358" alt="image" src="https://github.com/user-attachments/assets/790c10b8-659d-4f1a-b837-d7dcc8cb451d" />

3. Identify Packed F1 Seasons – Years with Over 20 Races
Objective: Determine which seasons had the most races.


<img width="362" height="432" alt="image" src="https://github.com/user-attachments/assets/9510670b-c5f9-41fc-be02-33ebe2995d14" />

4. Identify Drivers with Over 200 Career Points
Objective: List drivers who accumulated more than 200 points in their careers.


<img width="228" height="612" alt="image" src="https://github.com/user-attachments/assets/199fd75f-4b56-429e-8131-322f139ec9a5" />

5. Find Races Held at High-Altitude Circuits (Above 800 Meters)
Objective: Identify races held on circuits with challenging altitudes


<img width="452" height="720" alt="image" src="https://github.com/user-attachments/assets/1f74b1a2-8608-425e-9e72-59b8d6a2159d" />

6. Categorize Driver Performance Tiers Based on Career Points
Objective: Rank drivers by their career points.


<img width="602" height="736" alt="image" src="https://github.com/user-attachments/assets/bdaf5a10-63e7-464c-88c8-a4307413e0eb" />

7. Categorize Constructors by Region Based on Nationality
Objective: Group constructors into European or Non-European regions.


<img width="596" height="712" alt="image" src="https://github.com/user-attachments/assets/2088c5a2-3a3c-41f9-b9a9-c78295c0e0b5" />

8. Identify Drivers Who Never Raced for Ferrari
Objective: Find drivers who participated in races but never drove for a specific constructor.


<img width="376" height="728" alt="image" src="https://github.com/user-attachments/assets/2bfc167c-47d5-4fb1-89bd-6b2f1be06a14" />

9. List Races Held on Circuits in the UK
Objective: Identify races hosted at UK circuits.


<img width="386" height="206" alt="image" src="https://github.com/user-attachments/assets/6c70d819-9863-4afc-830c-f1af0c53a4b0" />

10. Calculate Average Points Per Race for Top Drivers
Objective: Determine which drivers perform best on average per race.


<img width="808" height="722" alt="image" src="https://github.com/user-attachments/assets/be38f7fb-81bd-4746-8f92-8402b288bd43" />

11. Find the Most Common Race Status
Objective: Identify the top 5 most frequent race outcomes.


<img width="358" height="270" alt="image" src="https://github.com/user-attachments/assets/46e05018-68cd-4285-819c-57e36e6eebdf" />

12. Calculate Average Lap Times for Drivers Who Won at Least One Race
Objective: Determine how winning drivers perform on average per lap.


<img width="358" height="582" alt="image" src="https://github.com/user-attachments/assets/8ee37c97-ba28-442c-b8b9-b33313142c70" />

13. Identify Constructors' First Win Year
Objective: Find the first year each constructor won a race.


<img width="460" height="572" alt="image" src="https://github.com/user-attachments/assets/3e8b17c3-b59b-49bb-9ac9-621f568c9ce7" />

14. Identify Peak Performance Seasons
Objective: Determine the seasons with the highest points scored by any constructor


<img width="354" height="262" alt="image" src="https://github.com/user-attachments/assets/fe8c9f5e-1e19-4972-89f1-9c1bf55f95a3" />

---

## Analysis & Visualizations 

Results and Insights

The Formula 1 data analysis combined 14 SQL queries with Excel visualisations to identify historical trends in driver performance, constructor success, race evolution, and circuit characteristics. The findings demonstrate how SQL can be used to extract meaningful insights from a large relational database.

Race Distribution Over Time

The analysis of races by decade (Figure 1) showed that the number of Formula 1 races has increased considerably since the championship began. Early decades contained relatively few races, while recent decades recorded substantially more events due to the global expansion of the sport.


<img width="500" height="464" alt="image" src="https://github.com/user-attachments/assets/a25ed567-4c2c-4d61-b5c6-df816c51a7c7" />

Figure 1. Number of Formula 1 races held in each decade


This trend is reinforced by the analysis of races per season, which identified multiple modern seasons containing more than 20 races, highlighting the increasing size of the Formula 1 calendar.

Constructor Performance

The constructor analysis revealed that only a small number of teams have consistently dominated Formula 1 over multiple decades. Several constructors recorded more than 100 race victories, demonstrating long-term competitiveness and sustained success.

Additional analysis identified the first year each constructor achieved a race win and the highest-scoring constructor for each season, illustrating how team performance has evolved throughout Formula 1 history.

Driver Performance

Driver statistics were analysed using total career points, average points per race and race participation.

The analysis found that:

Several drivers accumulated more than 200 career points, placing them among the sport's highest-performing competitors.
Average points per race highlighted drivers who consistently achieved strong race results rather than simply competing in a large number of events.
Drivers were successfully classified into performance tiers using SQL CASE statements, allowing comparisons between elite, intermediate and developing competitors.
Drivers who had never raced for Ferrari were also identified, demonstrating the use of exclusion queries and subqueries.

Circuit Characteristics

Circuit analysis focused on location and altitude.

The results identified several races held on circuits located above 800 metres, which represent relatively uncommon racing environments that can influence engine performance and race strategy.

The analysis also identified races hosted at United Kingdom circuits, illustrating the geographical distribution of Formula 1 events.

Race Outcomes

Race result data showed that the majority of entries finished successfully, while retirements caused by accidents, mechanical failures, or other issues occurred less frequently.

The five most common race statuses provided useful insight into the reliability of Formula 1 cars and the typical outcomes experienced during races.

Additional Performance Analysis

Further SQL queries expanded the analysis by examining:

Average lap times for drivers who had won at least one Formula 1 race.
Peak constructor performance by season based on total championship points.
Historical patterns linking constructors, drivers, and race outcomes across multiple decades.

These analyses demonstrated the ability to combine multiple relational tables using SQL JOIN operations and aggregate functions to answer complex analytical questions.

Summary of Key Findings

The project produced several important insights:

Formula 1 has expanded significantly, with modern seasons frequently containing more than 20 races.
Several constructors have achieved over 100 race wins, demonstrating long-term dominance.
Multiple drivers accumulated over 200 career points, distinguishing them as elite performers.
High-altitude circuits are relatively rare but represent unique racing environments.
Race status analysis highlighted the most common reasons for successful finishes and retirements.
SQL techniques such as JOINs, aggregations, CASE statements, and subqueries enabled the analysis of complex relationships across multiple database tables.

The accompanying Excel charts and summary tables complemented the SQL analysis by presenting historical trends in a clear and accessible format, making the findings suitable for both technical and non-technical audiences.

---

## Conclusion: 

Summary of the Analysis

This project successfully analysed a historical Formula 1 relational database using SQL (MySQL) and Excel to uncover trends in driver performance, constructor success, race calendar evolution, and circuit characteristics. Through data cleaning, exploratory data analysis (EDA) and the development of 14 SQL queries, the project transformed large volumes of historical race data into meaningful insights that were communicated through summary tables and visualisations.

Key Insights and Takeaways

The analysis revealed several important findings:

A small number of constructors have maintained long-term dominance, with several teams achieving more than 100 race wins.
Multiple drivers accumulated over 200 career points, highlighting consistent high performance throughout their careers.
Formula 1 seasons have expanded significantly over time, with many modern championships featuring more than 20 races.
High-altitude circuits are relatively uncommon but represent unique racing environments that may influence race performance.
Analysis of race statuses provided insights into common race outcomes and vehicle reliability.

These findings demonstrate the value of using SQL to identify historical trends and patterns within a large relational dataset.

Implications for Decision-Making

The analysis illustrates how historical performance data can support data-driven decision-making in motorsport. Teams could use similar analyses to benchmark their performance against competitors, evaluate driver consistency, identify successful long-term strategies and assess how circuit characteristics may influence race outcomes. Sports analysts and journalists could also use these insights to compare teams, drivers and seasons across different eras.

Recommendations for Future Analysis

Several opportunities exist to extend this project:

Incorporate additional data such as qualifying results, weather conditions, tyre strategies, pit stop information and championship standings.
Develop interactive dashboards using Power BI or Tableau to enable users to explore the data dynamically.
Apply predictive analytics or machine learning techniques to forecast race outcomes, driver performance, or constructor success.
Expand the analysis to investigate factors affecting reliability, championship-winning strategies and performance across different circuit types.

These enhancements would provide deeper insights into Formula 1 performance while further demonstrating advanced data analysis and visualisation skills.

---

## Credits

- **Collaborators:** Name – [GitHub Profile](https://github.com/USERNAME)  
- **Dataset Source:** [Link](https://link-to-dataset.com)  

---

## License

This project is licensed under the [MIT License](https://choosealicense.com/licenses/mit/) – feel free to use and modify it.  

---

<p align="center"><strong>Thanks for visiting! 🚀</strong></p>
