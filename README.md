CYBERSECURITY LEGISLATION IN UNITED STATES 
DATA CLEANING


WORKFLOW 1: PIVOT 
Input File: Legislation ID by year
Workflow: Pivot columns to rows
Output: Legislation_year.csv

WORKFLOW 2: UNION AND JOIN 
Input Files: 4 excel files per region + 1 legislation_year from workflow 1 (Converted to excel)
Workflow: Union region files, join legislation_year file
Output: RawData.csv
- Connect all the files using their region numbers which every file has.
- Connect all the files using union and add the converted excel file from workflow one to join.
- The files then are joined using their Legislation Number and the additional columns will now be connected to united file. Run flow in order to get the united and joined data data file.

WORKFLOW 3:
Input Files: RawData.csv
Workflow: Logical conditions, Mathematical fields, String related operations
Output: RawData.csv
- Logical Conditions:
Converting Division numbers to division names, region numbers to region names, State Cybersecurity Task Force (SCTF) type converting if it’s legislative, executive or no information stated.
- String Related Operations:
Splitting the State column (State name & State ID), changing State name to uppercase, changing state ID to uppercase, changing data types (Year to date, Legislation ID to String), Removed extra fields not needed.
- Mathematical Fields:
Calculated column: getting the sum of Total Cyber Security Legislations in the last 5 years, calculated column: getting the sum of total ransomware attacks in the last 5 years,  Ratios: Cybersecurity Legislations/Total Attacks
