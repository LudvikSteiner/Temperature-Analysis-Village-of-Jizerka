This is a R script performs a basic statistical analysis of temperature data collected in the village of Jizerka. The data include daily maximum, minimum, and average temperatures recorded over a given period.

Input Data
----------
- File: RDE.csv
- Format: CSV (Comma Separated Values)
- Expected Columns (after skipping the first row):
  1. Date
  2. Maximum temperature
  3. Minimum temperature
  
Note: Values are expected to use commas as decimal separators (e.g., "2,5").

What the Script Does
--------------------
1. Loads required libraries (readr, dplyr)
2. Reads the CSV file, skipping the first header row
3. Assigns column names: Date, Max, Min, and Average temperature
4. Converts character values to numeric, replacing commas with dots
5. Removes invalid rows (NAs caused by conversion)
6. Calculates summary statistics for each temperature type:
   - Mean
   - Trimmed mean (10%)
   - Median
   - Minimum and maximum
   - Standard deviation
   - Interquartile range (IQR)
7. Prints results to the R console
8. Exports the results to a new file temperature_statistics.csv

Output
------
- temperature_statistics.csv
  A single-row summary with statistics for:
  - Max_temperature
  - Min_temperature
  - Average

How to Run
----------
Make sure the RDE.csv file is located in your current working directory (check with getwd()), then run the script in RStudio or R terminal.

Requirements
-------------
Install packages
install.packages("readr")
install.packages("dplyr")
