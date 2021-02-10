# CYBERSECURITY LEGISLATION IN UNITED STATES 
A simple ETL project of a dataset using Tableau Prep + Final dashboard output.

## Business Problem
Connect datasets from different data sources and create a single dataset by joining the different data tables using Tableau Prep, after doing the ETL work, create a dashboard on the data.

## Solving the Problem

### WORKFLOW 1: 
Pivot columns to rows

### WORKFLOW 2: 
4 excel files per region + 1 legislation_year from workflow 1 (Union region files, join legislation_year file)
- Connect all the files using their region numbers which every file has.
- Connect all the files using union and add the converted excel file from workflow one to join.
- The files then are joined using their Legislation Number and the additional columns will now be connected to united file. Run flow in order to get the united and joined data data file.

### WORKFLOW 3: 
Logical conditions, Mathematical fields, String related operations
- Logical Conditions:
Converting Division numbers to division names, region numbers to region names, State Cybersecurity Task Force (SCTF) type converting if it’s legislative, executive or no information stated.
- String Related Operations:
Splitting the State column (State name & State ID), changing State name to uppercase, changing state ID to uppercase, changing data types (Year to date, Legislation ID to String), Removed extra fields not needed.
- Mathematical Fields:
Calculated column: getting the sum of Total Cyber Security Legislations in the last 5 years, calculated column: getting the sum of total ransomware attacks in the last 5 years,  Ratios: Cybersecurity Legislations/Total Attacks

Final presentation: https://public.tableau.com/profile/kathleen.lara#!/vizhome/Cybersecuirty/USCybersecuirtyLegislation
