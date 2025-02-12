# LAPD_SQL
LAPD Crime Data Analysis (SQL Project)

This project analyzes the LAPD crime dataset from 2023 to identify crime patterns and provide data-driven insights that can help resource allocation, policy recommendations, and crime prevention strategies. The dataset, sourced from Data.gov, contains information on crime incidents, locations, victims, weapons, and premises.

Using SQL queries with JOINs, subqueries, GROUP BY, HAVING, and aggregate functions, this project explores various aspects of crime in Los Angeles, including crime frequency, victim demographics, crime-heavy areas, weapon usage, and the most vulnerable premises.

Database Design & Normalization
To ensure efficiency and eliminate redundancy, the database was normalized to Third Normal Form (3NF). The original dataset contained nearly a million rows, which was too large to process effectively. Therefore, I filtered it down to only include incidents from 2023, reducing the dataset to 230,000 rows, allowing for more efficient querying while maintaining relevant insights.

Key normalization steps included:

Primary Table: The Incidents table serves as the central hub, connecting all other tables through foreign keys.
Separate Tables: Crime details, victims, weapons, and premises were stored in dedicated tables, reducing redundancy.
Elimination of Repeating Groups: Crime codes, weapon types, and locations were structured into separate tables using one-to-many relationships.
Foreign Keys for Data Integrity: Instead of inserting arbitrary IDs, I leveraged existing police codes for crime types, weapons, and locations to ensure consistency.
This approach optimized storage, improved query performance, and maintained data integrity, making it easier to analyze crime patterns.

Key Questions Explored & Findings
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
