# Pymaceuticals-challenge
Data on tumour volume (mm3) was compared between 10 active treatment arms (i.e., Capomulin, Ceftamin, Infubinol, Ketapril, Naftisol, Propriva, Ramicane, Stelasyn, and Zoniferol), as well as Placebo, over a period of up to 45 weeks in a murine model of squamous cell cancer.

## Project Description:
In the subfolder titled **data**, this project contains two separate .csv files:

1. **Mouse_metadata:**
Provides information on the ID, sex, age in months, and weight in grams of the 248 unique mice treated in this study.

2. **Study_results:**
Reports data on the ID, timepoint, tumour volume (mm3) and metastatic sites for each mouse up to 45 weeks.


## Installation and Run Instructions:
These two .csv files need to be merged together by executing the script provided in the **pymaceuticals_analysis_code** Jupyter Lab Notebook.


## Usage Instructions:
Following this, executing the script provided in the **pymaceuticals_analysis_code** Jupyter Lab Notebook will also output the following information:
 
  1. A dataframe summarising the mean, median, variance, standard deviation, and standard error of measurement of tumour volume (mm3) across all 10 arms.
  2. Bar charts summarising the number of mice treated in each treatment arm.
  3. Pie charts summaring mouse sex.
  4. Data on the 25% quantile, 50% quantile (median), and 75% quantile, as well as the upper and lower bounds, for tumor volume (mm3) for the four most promising active treatment arms (i.e., Capomulin, Ceftamin, Infubinol, and Ramicane) to enable the identification of potential outlier responses.
  5. Box plots summarising this information visually to enable the identification of potential outlier responses.
  6. A line graph summarising tumour growth (mm3) over time for a single mouse treated in the Capomulin arm.
  7. A scatter plot summarising the relationship between mouse weight in grams and tumour growth (mm3) for mice treated in the Capomulin arm.
  8. Pearson correlation coefficient for the relationship between mouse weight in grams and tumour growth (mm3) for mice treated in the Capomulin arm, and;
  9. Linear regression coefficient and plot for the relationship between mouse weight in grams and tumour growth (mm3) for mice treated in the Capomulin arm.


Types of merge options: https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.merge.html (accessed 21 March 2024).
Identifying duplicated entries: https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#duplicate-data (accessed 21 March 2024).
Aggregating function: https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.core.groupby.DataFrameGroupBy.agg.html (accessed 21 March 2024). 
Calculating summary statistics within groupby() function: https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.core.groupby.DataFrameGroupBy.mean.html (accessed 21 March 2024).
Advantage of idxmax() function over max() function to identify index of the entire row containing all data for the last recorded observation per mouse: https://stackoverflow.com/questions/60083433/what%C2%B4s-the-difference-between-idxmax-and-max-inside-a-groupby-pandas (accessed 22 March 2024).
