Hi there, I'm Drake!

I’m an analytics professional with a strong foundation in data analysis and storytelling, recently completing the Google Data Analytics Certificate through Merit America. My work focuses on turning complex datasets into clear, actionable insights—especially in sports and performance analytics.

**- Core expertise: data cleaning, exploratory analysis, metric design, visualization, and translating complex datasets into clear, actionable insights**

**- Technical strengths: SQL and R for analysis and modeling, Excel for structured reporting and Dashboard visualization.**

**- Ask me about: data analytics, data storytelling, wine trends, or how the right blend through data can change everything**

**- Career milestone: Completed the Google Data Analytics Certificate through Merit America and officially launched my career in analytics**

**- Long-term goal: become a Data Scientist**

**- Reach me at: dsoltez13@gmail.com**

**- Fun fact: I used to teach wine education—now I apply that same passion for discovery, pattern recognition, and storytelling to data analytics**

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# My Projects through Merit America:
## 🏈 R Project — Quarterback Decision Efficiency Case Study (2021–2024)

🔗 Repository: https://github.com/dsoltez/qb_decision_efficiency_case_study

## Summary

- This project evaluates quarterback decision-making using a custom-built Decision Efficiency Index (DEI) and multiple supporting metrics. Using NFL play-by-play data and Next Gen Stats (NGS), the analysis identifies which quarterbacks make the most effective decisions, how their performance trends over time, and whether quicker processing leads to better outcomes.
All results are visualized in R and compiled into a full R Markdown report.

## Dataset Sources

- NFL Play-by-Play Data (2021–2024) — via nflreadr / nflverse

- Next Gen Stats (Passing Data) — average time to throw, touchdowns, EPA, etc.

- Custom summary tables generated during processing:

    - Season-level QB summary

    - Combined four-season datasets

    - DEI-ranked datasets (4-season qualified & minimum 1-season QBs)

## Tools Used

- R / RStudio

- tidyverse, nflreadr, nflverse, ggplot2, viridis, ggrepel

- R Markdown for the final report

- GitHub for version control and documentation

## Steps I Took
### 1. Set Up the Decision Efficiency Index Environment

 - Built a reproducible analytical environment using the custom qb_setup.R script

 - Automatically installed & loaded all required R packages

 - Resolved package conflicts using {conflicted}

 - Loaded all NFL play-by-play and Next Gen Stats datasets with status messages

 - Ensured anyone can recreate the entire analysis by running:

    - source("qb_setup.R")

### 2. Imported & Cleaned All NFL Data

- Imported NFL play-by-play (2021–2024) and NGS passing data

- Filtered strictly for quarterback dropbacks

- Removed designed runs and invalid / non-passing plays

- Standardized quarterback names for reliable merging

- Cleaned key variables such as EPA, time-to-throw, and turnovers

### 3. Built the Decision Efficiency Index (DEI)
  - A custom composite metric blending:

      - Decision rate

      - EPA

      - Touchdowns

      - Turnover rate

      - Time-to-throw (decision tempo)

### 4. Analyzed all 4 Key Questions

- Q1: Which quarterbacks had the highest decision rate (percentage of effective decisions per dropback)?
- Q2: Which quarterbacks make consistently high-impact decisions (DEI)?
- Q3: Which quarterbacks show improvement or decline in decision efficiency over the four seasons?
- Q4: Is there a relationship between decision effectiveness and decision tempo (time to throw)?

### 5. Created polished visualizations

- Top 10 QB Decision Rate

- Top 10 DEI (4-year qualified)

- Top 10 DEI (min 1 season)

- Decision efficiency trends

- Decision effectiveness vs. tempo (regression scatterplot)

- Compiled everything into a final HTML report
  - (qb_decision_efficiency_case_study.html)

## Key Findings

- Mahomes, Tua, and Goff lead the league in decision rate over 2021–2024.

- DEI highlights Mahomes, Allen, and Tua as the most complete multi-year decision makers.

- Some young QBs (Purdy, Love) rank extremely high in DEI despite limited seasons.

- The negative correlation between time-to-throw and decision effectiveness indicates:

- Quarterbacks who process faster generally perform better.

- Veteran legends (Brady, Rodgers) still show elite decision-making late into their careers.

## Future Enhancements/Projects

- Expand the DEI to a 10-season dataset

- Compare DEI to traditional QB metrics (EPA/play, QBR, CPOE)

- Add situational DEI metrics (3rd down, red zone, 2-minute drill)

- Integrate pressure data into decision tempo

- Build a Shiny App for interactive DEI exploration

- Extend the framework to other sports or positions (WRs, RBs, DBs)

## About the DEI Metric

The Decision Efficiency Index (DEI) is a brand-new, custom, multi-factor QB metric developed specifically for this project.
It is currently in its early stages, and will evolve as new variables, weights, and data sources are incorporated.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# SQL Project — Global Layoffs Analysis (2020–2023)
## 🔗 Repository: https://github.com/dsoltez/global-layoffs-analysis
# 1. Summary:
This project analyzes global layoffs from 2020–2023 using SQL for data cleaning and exploratory analysis, followed by Excel for dashboard visualization. I cleaned and aggregated the dataset to uncover trends across companies, industries, countries, and yearly totals, then built an executive‑style dashboard to present the findings clearly and visually.
Dataset Source:
Kaggle — Global Layoffs Dataset (2020–2023)
## 2. Tools Used:
- SQL (data cleaning, aggregation, EDA)
- Excel (dashboard design, KPI cards, charts, filled map)
- CSV exports for structured outputs
- GitHub for version control and documentation
## 3. Steps I Took:
- Cleaned the raw dataset using SQL (duplicate removal, standardization, date formatting)
- Aggregated layoffs by company, industry, country, and year
- Performed exploratory analysis to identify top 10 companies and industries
- Generated country‑level and year‑over‑year summaries
- Exported cleaned and aggregated results as CSV
- Built a multi‑visual Excel dashboard (KPI cards, bar charts, map, line chart)
- Organized the project into data/, sql/, and visual/ folders with a structured README
## 4. Findings:
- 2022 had the highest total layoffs globally
- The United States accounted for the largest share of layoffs
- Amazon recorded the highest total layoffs among all companies
- Tech‑related industries dominated the top 10 most impacted sectors
- Layoffs rose sharply from 2020 to 2022 before stabilizing
## 5. Future Questions:
- How do layoffs correlate with macroeconomic indicators (inflation, interest rates)?
- Which industries recovered fastest post‑2023?
- Are layoffs concentrated in specific company sizes or revenue tiers?
- How do layoffs differ between tech and non‑tech sectors over time?
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
### SQL Project — BigQuery Homelessness Analysis
🔗 **Repository:** https://github.com/dsoltez/bigquery-sql-homelessness-analysis

**Summary:**  
This project explores U.S. homelessness data using Google BigQuery SQL. I analyzed patterns in total homelessness, unsheltered populations, youth homelessness, and state-level differences, then exported the results to CSV and organized them in a structured GitHub repository.

**Dataset Source:**  
BigQuery Public Dataset — `bigquery-public-data.sdoh_hud_pit_homelessness.hud_pit_by_coc`

**Tools Used:**  
- Google BigQuery (SQL querying)
- CSV export for local analysis
- GitHub for version control and organization

**Steps I Took:**  
1. Connected to BigQuery’s public homelessness dataset  
2. Filtered and grouped data by state (2018)  
3. Segmented by total homeless, unsheltered homeless, and youth homeless  
4. Created multiple SQL queries to answer targeted questions  
5. Exported results as CSV  
6. Organized work into `data/`, `sql/`, and `docs/` folders  
7. Summarized insights in the README  

**Findings:**  
- California, New York, and Florida had the highest total homelessness  
- Several states exceeded 1,000 unsheltered individuals, suggesting infrastructure strain  
- Some states had less than 2% unsheltered homelessness, indicating strong shelter systems  
- Youth homelessness concentrated primarily in population-dense states  
- Delaware showed atypical ratios compared to national patterns  

**Future Questions:**  
- How does climate influence unsheltered homelessness?  
- Do shelter investments reduce unsheltered percentages?  
- How do eviction policies affect homelessness trends?  
- How does cost-of-living correlate with total homelessness?

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------



------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

![Excel](https://img.shields.io/badge/Excel-Data%20Analysis-informational?style=flat&logo=microsoft-excel&logoColor=white&color=217346)
![SQL](https://img.shields.io/badge/SQL-Queries-blue)
![Tableau](https://img.shields.io/badge/Tableau-Dashboards-orange)
![R](https://img.shields.io/badge/R-Programming-blue)
![GitHub](https://img.shields.io/badge/GitHub-Version%20Control-black)
