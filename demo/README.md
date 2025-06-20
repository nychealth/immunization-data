This folder contains vaccination data stratified by demographic types. 

Vaccination coverages with numerators COUNT_PEOPLE_VAC less than 10 (9 or fewer) are suppressed and not shown due to small numbers. Vaccination coverages with denominators less than 50 should be interpreted with caution due to small population estimates. 

*Main_Routine_Vaccine_Demo.csv*

Variables include: 

|Variable Name | Definition |
|---|---|
DATE_CREATED | Date of data retrieved from the CIR
AGE_GROUP |Age group 
DOB_RANGE |Date of birth range for cohort population estimates 
VACCINE_GROUP |Vaccine series 
DOSES |Number of doses 
YEAR_COVERAGE |Year of vaccination coverage  
QUARTER |Quarter of vaccination coverage, in calendar year
RACE_ETHNICITY |Combined race and ethnicity 
POP_DENOMINATOR_YEAR |Year of population estimates 
POP_DENOMINATOR |Population estimates, denominator for vaccination coverage 
COUNT_PEOPLE_VAC |Number of people who received the number of recommended doses of the vaccine series, numerator for vaccination coverage 
PERC_VAC |Point estimates of vaccination coverage, percentage rounded to the nearest whole number, capped at 99% of the population who received the number of recommended doses of the vaccine series
