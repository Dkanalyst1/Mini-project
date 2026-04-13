<img width="940" height="470" alt="image" src="https://github.com/user-attachments/assets/33932df6-9004-4f9d-b994-d67627577c4a" /># Mini-project
About Identifying key factors that influenced election victories or defeats across various states. Measuring turnout percentages to determine public engagement levels. Analyzing performance based on category and gender. Hence this project analyzes assembly election data across multiple Indian states.

     PROJECT OVERVIEW AND OBJECTIVE
        This project involves cleaning, transforming, and analysing raw data using Excel and creating an interactive Power BI dashboard to derive meaningful business insights.
          The main objective is to demonstrate data pre-processing techniques using Excel and an interactive Power BI dashboard visualization to make informed decisions.
     DATA SOURCES
        Source Description and Timeline: India Data Portal: https://indiadataportal.com/  Search and 2009-2021. 
 Domain: Politics (Election).

PROBLEM STATEMENT
 
Understanding Election Outcomes:
Identifing the key factors that influenced victory or defeat across different states and constituencies.
     Analyzing Voter Participation:
Measuring voter turnout percentages to determine public engagement levels in various election cycles.
     Evaluating Candidate Diversity:
Analyzing the performance of candidates based on their category (General, SC,ST) and gender to understand representation.
     Assessing Victory Margins:
Identifying “close-contest” seats versus “safe” seats by calculating the average winning margin percentage.
     Tracking Historical Trends: 
             Monitoring how voting patterns and total votes obtained have changed over time using historical election dates.
ATTRIBUTE (COLUMN/FEATURES) DETAILS:
Attributes	Data Type	Description
Election Date	Date	The Specific date when the election was held.
State Name	Text	Name of the Indian State where the constituency is located.
Assembly No	Whole Number	The official constituency number assigned by the Election commission.
Assembly Constituency Name	Text	The Specific name of the legislative assembly seat (e.g., Thousand Lights).
Candidate Name	Text	Name of the individual contestant in the election.
Candidate Type	Text	Categorization of candidates based on reservation (General, SC,ST).
Sex	Text	Gender of the candidate (Male,Female,Others).
Party	Text	Political Party affiliation of the candidate.
Position	Whole Number	Final rank of the candidate based on votes(1 = winner).
Total Votes Obtained	Decimal Number	Total number of valid votes secured by the candidate.
Margin Percentage	Percentage	The difference in vote share between the candidate and the runner-up.
Turn out Percentage	Percentage	The percentage of total electors who actually cast their votes.

TOOLS & TECHNOLOGIES
  ● Excel: Data cleaning, transformation, and Pivot Tables. 
  ● Power BI: Data modelling, DAX calculations, visualization, and interactive dashboard creation.
DATA PRE-PROCESSING (EXCEL/POWER QUERY)
Tasks Performed:
 ● Data Cleaning & Transformation: Removed duplicates, handled missing values, standardized formats, and created calculated fields.
 ● Filtering & Sorting: Organized data to focus on relevant records.
 ● Pivot Tables: Generated Pivot Tables for data summarisation and initial insights.
 ● Convert the data into Fact and Dimension Table 
DATA MODELLING AND DAX (POWER BI)
● Data Model: Connected Dimension tables to a central Fact table via One-to-Many (1:*) links.

<img width="1334" height="665" alt="Screenshot 2026-03-03 110451" src="https://github.com/user-attachments/assets/815692ba-3e32-4b44-
a2fd-8f6b917d74bd" />

DAX Measures: 
  Total Votes: SUM(‘Assembly Elections Data’[Sum of Total Votes Obtained])
  Avg Margin %: AVERAGE (‘Assembly Elections Data’ [Margin Percentage])

ANALYSIS AND VISUALIZATIONS (POWER BI)
1.Core KPI Cards:
Instruction:Use the Card Visual for single high-level metrics.
Insights: Highlights the overall health of the election data, such as 7M Total Votes and 4.28% Average Margin. It gives an immediate summary of the scale and competitiveness of the elections.

<img width="940" height="466" alt="image" src="https://github.com/user-attachments/assets/14c3c7ea-50ef-490e-98ce-2c7868c12f26" />

2.Gender & Category Bar Charts:
    Instruction: Use clustered Bar chart to compare two different groups like ‘sex’ or ‘Candidate Type’.
    Insight: This diagram helps identify which demographic (e.g., Male vs Female) has the highest Vote Share Percentage explains the “Why” behind a party’s performance in specific voter segments.

<img width="940" height="466" alt="image" src="https://github.com/user-attachments/assets/41152096-6765-4332-afc9-ed8b97e04295" />

3.Constituency Distribution (Trend/Structural Insight):
    Instruction: Use a Tree Map to visualize the volume of constituencies per state. 
    Insights: The size of the boxes indicates which states have more administrative seats (e.g., Uttar Pradesh vs Manipur). This helps in understanding the political weight of  each state in the overall analysis.

<img width="940" height="475" alt="image" src="https://github.com/user-attachments/assets/ce21a239-295d-47bb-bac4-08963d7a0c6c" />

 4. Detailed Elector Analysis (Performance Insight)
    Instruction: Use a Stacked Bar Chart with the Zoom Slider enabled for large datasets.
    Insight: Shows the total electors for every constituency. By using the zoom slider, users can focus on specific high-population areas without losing the context of the entire dataset.

<img width="940" height="470" alt="image" src="https://github.com/user-attachments/assets/657f4497-857a-496d-8568-1cd1d7ba4cca" />


INSIGHT & CONCLUSIONS
OVERVIEW

<img width="940" height="467" alt="image" src="https://github.com/user-attachments/assets/18ddce3f-423f-48a1-a06f-e7e57773166c" />

Key Findings: High scale, Tight Contests, Male Dominance, State weight, Voter variation.
Analysis Insights:
●	Summarizes the actual results of the election.Shows key figures like Total Votes (7M) and Average Margin % (4.28%).
●	Investigates why certain results happened by looking at categories. Compares data across Candidate Types (General,SC,ST) and Gender (Male/Female) to see which group influenced the win.
●	Measures how strong the winners were in each constituency. Identifies “Safe Seats’ (high margin) versus “Close Contests” (low margin) using DAX Measures.
●	Tracks how voting patterns changed over time. Uses the Election Date to show if voter turnout is increasing or decreasing across different years.
 
CONCLUSIONS
       The integration of Excel and Power BI proved effective for end-to-end data analysis, from raw data to visual reporting.

















