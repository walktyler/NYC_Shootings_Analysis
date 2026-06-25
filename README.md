# NYC_Shootings_Analysis
Developed an interactive Power BI dashboard to analyze over 18 years of NYPD shooting incident data. The project explores temporal patterns, borough-level trends, year-over-year changes, seasonality, and shooting hotspots throughout New York City. Through data modeling, SQL based transformations, and visual analytics, the dashboard enables stakeholders to monitor public safety trends, identify periods of elevated risk, and evaluate how shooting activity has changed across NYC neighborhoods over time.  

# Project Background
The Shootings dataset contains detailed records about shooting incidents recorded by the New York City Police Department, where each row represents a single shooting incident. This dataset contains shooting incidents from 2006 to present day, being updated quarterly.

Insights and recommendations are structured around the following analytical themes:
1) ### Time and Risk Patterns
- During which months do shootings occur most frequently?
- Which times of day experience the highest concentration of shootings?
- Are there seasonal patterns in shooting activity?
2) ### Trend Analysis
- How have shooting incidents changed over time?
- Which years experienced significant increases or decreases?
- Has public safety improved or worsened over the past two decades?
3) ### Borough Level
- Which boroughs experience the highest number of shootings?
- Which precincts report the most incidents?
- How has shooting activity changed across boroughs over time?
4) ### Public Safety Monitoring
- What recent trends should stakeholders monitor?
- Which areas may require additional intervention or resources?


# Data Structure
Data Source [here](https://data.cityofnewyork.us/Public-Safety/Shootings-2006-Present-/5ucz-vwe8/about_data)

The Data Structure for RAW_NYC_Shootings is as shown, totaling 24,127 rows.

<img width="249" height="565" alt="image" src="https://github.com/user-attachments/assets/33252567-e0b8-49b8-820e-5f70172f870b" />

# Data Cleaning & Preparation
Prior to analysis, comprehensive data quality checks and cleaning were performed:
- Imported source data into Microsoft SQL Server.
- Verified incident uniqueness using INCIDENT_KEY.
- Reviewed data types and corrected formatting inconsistencies.
- Assessed completeness and identified missing values.

# Data Transformation
- Extracted Year, Month, Day of Week, and Hour from occurrence dates and times.
- Created Time-of-Day categories:
  - Morning
  - Afternoon
  - Evening
  - Night
- Developed Year-over-Year Growth Rate measures.
- Created seasonal aggregations to support trend analysis.

# Data Quality Results
- No duplicate incident records identified.
- Borough and precinct values were standardized.
- Missing values were reviewed and determined not to materially impact the analysis.

# Executive Summary
### Overview of Findings
Analysis of more than 24,000 shooting incidents revealed several notable trends:

### Long-Term Decline with a Temporary Surge
Shooting incidents generally declined between 2006 and 2019. However, incidents increased sharply during 2020, reaching 1,562 shootings, representing a 97.2% increase from the previous year.
Following this surge, shootings resumed a downward trend, with the most recent full year experiencing a 23.9% decrease compared to the prior year.

### Strong Seasonal Patterns
Shooting incidents peak during the summer months, particularly June through August. July recorded the highest number of incidents among all months analyzed.

### Nighttime Represents the Highest Risk Period
Nearly half of all shootings occurred during nighttime hours, making it the most common period for shooting incidents.

### Brooklyn Accounts for the Largest Share of Shootings
Brooklyn recorded 9,726 incidents, representing the highest total among all boroughs. The Bronx ranked second with 6,979 incidents.

### Concentration Among Specific Precincts
A small number of precincts account for a disproportionate share of incidents, with Precincts 75 and 73 in Brooklyn recording the highest shooting volumes citywide.

<img width="2121" height="1186" alt="image" src="https://github.com/user-attachments/assets/87e6ed7c-166a-4d71-a81a-bf34fc7f8806" />



# Recommendations

### Target Summer Violence Prevention Efforts
- Because shootings consistently increase during summer months, public safety initiatives should be concentrated between May and August when risk is highest.

### Prioritize Nighttime Enforcement and Outreach
- With nearly half of shootings occurring at night, resource allocation and intervention programs should focus on evening and overnight hours.
