# LAPD_SQL
LAPD Crime Data Analysis (SQL Project)

This project analyzes the LAPD crime dataset from 2023 to identify crime patterns and provide data-driven insights that can help resource allocation, policy recommendations, and crime prevention strategies. The dataset, sourced from Data.gov, contains information on crime incidents, locations, victims, weapons, and premises.

Using SQL queries with JOINs, subqueries, GROUP BY, HAVING, and aggregate functions, this project explores various aspects of crime in Los Angeles, including crime frequency, victim demographics, crime-heavy areas, weapon usage, and the most vulnerable premises.

Data Processing & CSV Breakdown:
To ensure efficiency and eliminate redundancy, I normalized the database to Third Normal Form (3NF). The original dataset contained nearly a million rows, which was too large to process effectively. Therefore, I filtered it down to only include incidents from 2023, reducing the dataset to 230,000 rows, allowing for more efficient querying while maintaining relevant insights.Before loading the data into SQL, I broke the original dataset into 7 separate CSV files, each corresponding to a different table in the database:

Incidents.csv – Core dataset containing all reported crimes.
Crime_Details.csv – Information on crime types and descriptions.
Victim_Details.csv – Demographic details of victims.
Weapons.csv – Weapons involved in incidents.
Locations.csv – Area names and identifiers.
Premises.csv – Types of locations where crimes occurred.
Status.csv – Incident status codes.
This approach ensured that data was structured relationally before importing into SQL, optimizing storage and query performance.

Raw SQL Dump & Code:
The raw SQL dump of the fully structured database can be found in:
📄 annotated-crime_data_LA-1.sql.pdf
The questions, SQL queries, and answers related to the analysis can be found in:
📄 Questions + Code + Answers.pdf

Key Questions Explored & Findings:
1. Crime Distribution by Area:
Central LA had the highest crime rate, followed by 77th Street, Pacific, and Southwest LA.
These areas should be the focus of targeted crime reduction strategies.
3. Most Common Crime Types:
The top 5 crimes in Los Angeles in 2023 were:
Vehicle Theft
Battery
Burglary
Identity Theft
Burglary from Vehicles
4. Crime Trends in High-Crime Areas:
Central LA: Burglary from vehicles, battery, and vehicle theft.
77th Street: Stolen vehicles, assault with a deadly weapon, and battery.
Pacific: Stolen vehicles, petty theft, and burglary.
5. Victim Demographics:
The average victim age was 29 years old.
Certain crimes, like grand theft and attempted theft from vehicles, involved older victims.
6. Weapons Used in Crimes:
Bodily force (without weapons) was the most frequently used method.
Handguns were strongly associated with robbery cases.
7. Crime Locations & Premises Insights:
Most crimes occurred on the street, in single-family dwellings, and multi-unit dwellings.
Street crimes mainly involved stolen vehicles and vehicle burglaries.
Identity theft was more common in residential areas.
Implication: The LAPD can use this insight for public awareness campaigns and crime prevention efforts
