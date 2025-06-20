This folder contains vaccination data stratified by geographic types. 

Vaccination coverages with numerators COUNT_PEOPLE_VAC less than 10 (9 or fewer) are suppressed and not shown due to small numbers. Vaccination coverages with denominators less than 50 should be interpreted with caution due to small population estimates. 

*Main_Routine_Vaccine_Geo.csv*

Variables include: 

|Variable Name |Definition|
|---|---|
DATE_CREATED | Date of data retrieved from the CIR 
AGE_GROUP | Age group 
DOB RANGE | Date of birth range for cohort population estimates 
VACCINE_GROUP | Vaccine series 
DOSES | Number of doses 
YEAR_COVERAGE | Year of vaccination coverage  
QUARTER | Quarter of vaccination coverage, in calendar year
BOROUGH | Name of borough 
MODZCTA | Modified ZCTA (ZIP Code Tabulation Area, which solidifies ZIP codes into units of area) 
LABEL | List of the ZIP Code Tabulation Areas (ZCTAs) that are bundled into the MODZCTA 
NEIGHBORHOOD_NAME | Neighborhood name of the MODZCTA 
POP_DENOMINATOR_YEAR | Year of population estimates 
POP_DENOMINATOR |Population estimates, denominator for vaccination coverage 
COUNT_PEOPLE_VAC |Number of people who received the number of recommended doses of the vaccine series, numerator for vaccination coverage 
PERC_VAC |Point estimates of vaccination coverage, percentage rounded to the nearest whole number, capped at 99% of the population who received the number of recommended doses of the vaccine series
