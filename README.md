# Childhood Vaccination Data 

This repository contains data on routine immunizations administered to New York City (NYC) children ages 0-18 years and reported to the [Citywide Immunization Registry](https://www.nyc.gov/site/doh/providers/reporting-and-services/citywide-immunization-registry-cir.page) (CIR). These data are available on the NYC Health Department’s Childhood Vaccination Data page.

**This Readme includes the following topics:**

- How to Use This Repository 
- Key Technical Notes 
- Definitions 
- Repository Contents 

## How to Use This Repository   

Two main datasets serve as the data sources for all the visualizations displayed on the Childhood Vaccination Data page on the NYC Health webpage. One dataset is stratified by individual demographics and the other is stratified by geography. Users can download a separate dataset for each visualization by clicking ‘Get the data’ under the visualization or by downloading the full dataset under **‘Repository Contents’.** 

## Key Technical Notes 

**Citywide Immunization Registry**

Since 1996, the [Citywide Immunization Registry](https://www.nyc.gov/site/doh/providers/reporting-and-services/citywide-immunization-registry-cir.page) (CIR) has been used as a database of patient immunization records reported by NYC health care providers and some out-of-state immunization information systems. The CIR keeps immunization records for all NYC residents – children and adults – throughout their lifespan and has records for non-NYC residents vaccinated in the city. It is accessible to authorized health care providers, schools, individuals and agencies concerned with public health to ensure that NYC residents are up to date with recommended immunizations. NYC health care providers report immunizations to the CIR as mandated by New York State Public Health Law and the NYC Health Code. Pediatric providers are required to report all immunizations administered to children 0-18 years. Reporting of adult immunizations requires patient consent. Immunization data are submitted to the CIR through electronic health record systems or the [CIR’s Online Registry](https://immunize.nyc/prod/online-registry/) user interface.

**Childhood Vaccination Data Update Schedule**

The Childhood Vaccination Data page displays vaccination coverage data for the past five years stratified by race and ethnicity and NYC neighborhood. Additionally, trends in citywide coverage are displayed for the past eight years. Data presented on the Childhood Vaccination Data page are updated twice a year, as of June 30 and December 31 of each year. Data are released one to two months after the coverage assessment date to allow enough time for data to be reported to the CIR and prepared for public sharing. 

Data are preliminary and subject to change when new population estimates are published. 

## Definitions 

**Age cohort**  (AGE_GROUP) <br>
The NYC Health Department tracks vaccination coverage among NYC children and adolescents in several age cohorts depending on vaccine series. 

- For the combined 7-vaccine series and each component vaccine, the Health Department tracks coverage for children ages 2 years by their second birthday which includes children between the ages of 24 months 0 day and 35 months 30 days as of the coverage assessment date. 
- For HPV, the Health Department tracks HPV series completion rates for 13-year-olds by their thirteenth birthday to monitor on-time vaccination at ages 11 to 12 years, and completion rates for adolescents ages 13 to 17 years. Adolescents ages 13 years include adolescents between the ages of 13 years 0 day and 13 years 11 months 30 days as of the coverage assessment date. Adolescents ages 13 to 17 years include adolescents between the ages of 13 years 0 day and 17 years 11 months 30 days as of the coverage assessment date.
- For influenza (flu) vaccination, the Health Department tracks coverage for children ages 6-months to 4-years, 5-to-12-years and 13-to-17-years. Since the influenza season spans multiple months, the age criterion for the analysis is based on the child’s age (in days) at the time of the flu vaccination. The CIR calculates a child’s age days by subtracting the child’s date of birth from the flu vaccination date. This includes children between the ages of 182 and 1,825 days (for the 6-month to 4-year-old cohort), between the ages of 1,826 and 4,747 days (for the 5-to–12-year-old cohort), and between the ages of 4,748 and 6,573 days (for the 13-to-17-year-old cohort) as of the coverage assessment date.

**Numerator** (COUNT_PEOPLE_VAC)  
The numerators include children in the CIR who meet the following criteria: 
- Received all required doses of the specified vaccines 
- Not documented in the CIR as having moved out of NYC or deceased 
- Had a valid NYC ZIP code listed in the CIR as of the coverage assessment date

Historical data of years 2017 to 2024 were pulled from the CIR on May 16, 2025. New data are pulled from the CIR one to two months after the coverage assessment date.

**Denominator** (POP_DENOMINATOR)  
The denominators for routine vaccination coverage and seasonal influenza vaccination coverage estimates are based on the most recent denominators (population estimates) available at the NYC Health Department. The NYC Health Department produces these estimates (called Vintage) using data from the U.S. Census Bureau and the NYC Department of City Planning. The Vintage year is the year the estimates were produced and usually with one year lag in the population estimate year. For example, Vintage 2022 includes population estimates for years 2000 to 2021. 

On the Childhood Vaccination Data page, the denominators for historical data of years 2017 to 2019 use respective population estimate years in Vintage 2022. The denominators for historical data of years 2020 to 2023 use respective population estimate years in DOHMH Vintage 2024. The denominators for year 2024 use the most recent population estimates available in year 2023 in DOHMH Vintage 2024. The denominators for new data use the most recent population estimates available. For details of the source of the denominators, please look at the two main datasets under ‘Repository Contents’. 

**Vaccination Rate** (PERC_VAC)  
Vaccination coverage is determined by taking the numerator (COUNT_PEOPLE_VAC) divided by the denominator (POP_DENOMINATOR). Vaccination coverage exceeding 99% are capped at 99%. Vaccination coverages with numerators less than 10 (9 or fewer) are suppressed due to small numbers. Vaccination coverages with denominators less than 50 should be interpreted with caution due to small population estimates. This may happen with small demographic and geographic categories. 

**Vaccine Groups** (VACCINE_GROUP)   
- [Childhood Combined 7-Vaccine Series (≥4 DTaP, ≥3 Polio, ≥1 MMR, ≥3 Hib, ≥3 HepB, ≥1 Varicella, ≥4 PCV)](#seven)
- [Diphtheria and Tetanus Toxoids and Acellular Pertussis Vaccine (DTaP/DT/DTP)](#dtap)
- [Poliovirus Vaccine (Polio)](#polio) 
- [Measles, Mumps and Rubella Vaccine (MMR)](#mmr) 
- [Haemophilus Influenzae Type b Vaccine (Hib)](#hib) 
- [Hepatitis B Vaccine (HepB)](#hepb) 
- [Varicella (chickenpox) Vaccine (VAR)](#var) 
- [Pneumococcal Conjugate Vaccine (PCV)](#pcv) 
- [Human Papillomavirus Vaccine (HPV)](#hpv)
- [Influenza Vaccine (Flu)](#flu) 
<br>
<span id="seven"></span>
Childhood Combined 7-Vaccine Series (≥4 DTaP, ≥3 Polio, ≥1 MMR, ≥3 Hib, ≥3 HepB, ≥1 Varicella, ≥4 PCV)

- The combined 7-vaccine series (also known as the 4:3:1:3:3:1:4 series) measures the percentage of children ages 2 years who received all required doses of the series by their second birthday. 

- The series includes ≥4 doses of diphtheria and tetanus toxoids and acellular pertussis vaccine; ≥3 doses of poliovirus vaccine; ≥1 dose of measles-mumps-rubella vaccine; ≥3 or ≥4 doses of *Haemophilus Influenzae* Type b vaccine (depending on product type); ≥3 doses of hepatitis B vaccine; ≥1 dose of varicella vaccine; and ≥4 doses of pneumococcal conjugate vaccine.  

- For more information about the 7-vaccine series and all CDC recommended vaccines, visit Birth-18 Years Immunization Schedule https://www.cdc.gov/vaccines/hcp/imz-schedules/child-adolescent-age.html 

<span id="dtap"></span>
Diphtheria and Tetanus Toxoids and Acellular Pertussis Vaccine (DTaP/DT/DTP) 

- The CDC maintains updated guidelines and recommendations on diphtheria, tetanus and pertussis vaccination (DTaP/DT/DTP). For more information, visit: 

  - https://www.cdc.gov/diphtheria/vaccines/index.html 
  - https://www.cdc.gov/tetanus/vaccines/index.html 
  - https://www.cdc.gov/pertussis/vaccines/index.html 
  
- Vaccination Tracking: Percent vaccinated is calculated by dividing the number of 24-35-month-olds who have received 4 or more doses of DTaP vaccine by their second birthday according to the CIR, by the total number of same-aged children in that year according to the most recent Vintage population estimates. 

<span id="polio"></span>
Poliovirus Vaccine (Polio) 

- The CDC maintains updated guidelines and recommendations on poliovirus vaccination. For more information, visit: https://www.cdc.gov/polio/vaccines/index.html   
- Vaccination Tracking: Percent vaccinated is calculated by dividing the number of 24-35-month-olds who received 3 or more doses of inactivated polio vaccine (IPV) by their second birthday according to the CIR, by the total number of same-aged children in that year according to the most recent Vintage population estimates. 

<span id="mmr"></span>
Measles-Mumps-Rubella Vaccine (MMR) 

- The CDC maintains updated guidelines and recommendations on MMR vaccination. For more information, visit:
  - https://www.cdc.gov/measles/vaccines/index.html
  - https://www.cdc.gov/mumps/vaccines/index.html
  - https://www.cdc.gov/rubella/vaccines/index.html
- Vaccination Tracking: Percent vaccinated is calculated by dividing the number of 24-35-month-olds who received one or more doses of MMR vaccine by their second birthday according to the CIR, by the total number of same-aged children in that year according to the most recent Vintage population estimates.

<span id="hib"></span>
*Haemophilus Influenzae* Type b Vaccine (Hib) 

- The CDC maintains updated guidelines and vaccine recommendations on Hib vaccination. For more information, visit: https://www.cdc.gov/hi-disease/vaccines/index.html 
- Vaccination Tracking: Percent vaccinated is calculated by dividing the number of 24-35-month-olds who received all required doses of Hib vaccine by their second birthday according to the CIR, by the total number of same-aged children in that year according to the most recent Vintage population estimates. 

<span id="hepb"></span>
Hepatitis B Vaccine (HepB) 

- The CDC maintains updated guidelines and vaccine recommendations on HepB vaccination. For more information, visit: https://www.cdc.gov/hepatitis-b/vaccination/index.html
- Vaccination Tracking: Percent vaccinated is calculated by dividing the number of 24-35-month-olds who received 3 doses of HepB vaccine by their second birthday according to the CIR, by the total number of same-aged children in that year according to the most recent Vintage population estimates. 

<span id="var"></span>
Varicella (chickenpox) Vaccine (VAR) 

- The CDC maintains updated guidelines and vaccine recommendations on varicella vaccination. For more information, visit: https://www.cdc.gov/chickenpox/vaccines/index.html
- Vaccination Tracking: Percent vaccinated is calculated by dividing the number of 24-35-month-olds who received one or more doses of varicella vaccine by their second birthday according to the CIR, by the total number of same-aged children in that year according to the most recent Vintage population estimates. 

<span id="pcv"></span>
Pneumococcal Conjugate Vaccine (PCV) 

- The CDC maintains updated guidelines and recommendations on pneumococcal vaccination. For more information, visit: https://www.cdc.gov/pneumococcal/vaccines/index.html
- Vaccination Tracking: Percent vaccinated is calculated by dividing the number of 24-35-month-olds who received all required doses of PCV by their second birthday according to the CIR, by the total number of same-aged children in that year according to the most recent Vintage Population estimates. 


<span id="hpv"></span>
Human Papillomavirus Vaccine (HPV) 

- The CDC maintains updated guidelines and recommendations on HPV vaccination. For more information, visit: https://www.cdc.gov/hpv/vaccines/index.html 
- Vaccination Tracking: Percent vaccinated is calculated by dividing the number of 13-17-year-olds who received all required doses of HPV vaccine according to the CIR, by the total number of same-aged adolescents in that year according to the most recent Vintage Population estimates. On-time vaccination is calculated by dividing the number of 13-year-olds who completed the HPV vaccine series by their thirteenth birthday according to the CIR, by the total number of 13-year-olds in that year according to the most recent Vintage Population estimates.  

<span id="flu"></span>
Influenza Vaccine (Flu) 

- The CDC maintains updated guidelines and recommendations on flu vaccination. For more information, visit: https://www.cdc.gov/flu/vaccines/index.html 
- Vaccination Tracking: Percent vaccinated is calculated by dividing the total number of children who received at least one seasonal flu vaccine during the target flu season according to the CIR, by the total number of same-aged children in that year according to the most recent Vintage population estimates. Patient age criterion is based on the patient’s age (in days) at the time of the flu vaccination.  

## Demographic Variables 
A large proportion of the vaccination data reported to the CIR come from proprietary health care provider electronic health record (EHR) systems that are not managed by the NYC Health Department. Data in the CIR are limited to what is available in EHR systems and to the fields required for submission. Information on demographics, such as race and ethnicity can be incomplete.  

**Race and Ethnicity** (RACE_ETHNICITY)  
The CIR collects race and Hispanic/Latino ethnicity separately. For determining vaccination coverages for the NYC population in this data repository, CIR combines and classifies the proportion of people vaccinated by race/ethnicity into the following mutually exclusive categories: Asian, Black/African American, Hispanic/Latino, and White. The Hispanic/Latino category includes people of any race, and all other categories exclude those who identify as Hispanic/Latino. Disaggregated information on vaccinations among people identified as American Indian/Alaska Native, Native Hawaiian or other Pacific Islander, and two or more races are provided only as counts due to smaller numbers for these groups. Race/ethnicity coverage data should be interpreted with caution when comparing to citywide coverage. 

**ZIP Codes** (MODZCTA)  
We report information by geography using modified ZIP Code Tabulation Areas (MODZCTA) based on the ZIP code of residence reported by the vaccine recipient at the time of vaccination. A ZIP code does not refer to a specific area, but rather a collection of addresses that make up a mail delivery route. To represent the area that the route is in, the U.S. Census Bureau developed ZIP Code Tabulation Areas (ZCTAs). In ZCTAs, some ZIP codes are bundled together into a single ZCTA. 

Modified ZCTA (MODZCTA) is a geographic unit used to analyze health data. ZCTAs with small populations are combined into Modified ZCTAs to allow for stable rate calculations by increasing the underlying population of these areas. See [Modified ZIP Code Tabulation Areas NYC webpage](https://nychealth.github.io/covid-maps/modzcta-geo/about.html) to identify in which MODZCTA a ZIP code is. 

The number of people vaccinated in some neighborhoods may exceed the estimated population. The percentage of people vaccinated is calculated using intercensal population estimates from the most recent population estimates produced by the NYC Health Department. When new yearly population estimates are released each year, vaccination coverage by geography will be adjusted accordingly using the same numerators and the new population estimates. Vaccination coverages using previous population estimates are archived.  

Additional factors contributing to these inconsistencies may be that self-reported ZIP code at the time of vaccination may not correspond to the recipient’s primary home address. For example, people may use their school dormitory or work address. Individuals whose addresses are not valid and, therefore, cannot be mapped to a MODZCTA are not included in the maps or data download.  
## Suggested Citation 
New York City Department of Health and Mental Hygiene. Childhood Vaccination Data. Data as of [VERSION DATE]. Accessed at [LINK] on [ACCESS DATE]. <br>   

## Repository Contents 

**demographic/**
This folder contains vaccination data stratified by demographic types. 

**geographic/**
This folder contains vaccination data stratified by geographic types. 

**visualizations/**
This folder contains separate datasets for each visualization on the NYC Health Department's Childhood Vaccination Data page.
