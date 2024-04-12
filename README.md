# Crunching Numbers, Saving Lives: Road Safety Analysis 2021–2022

## Introduction
Road accidents pose a significant threat to public safety, and understanding their dynamics is crucial for implementing effective preventive measures. In the United Kingdom, the Department for Transport (DfT) meticulously collects and analyzes data on traffic casualties through the Reported Road Casualties Great Britain (RRCGB) publication. This official statistical repository offers invaluable insights into the trends, patterns, and contributing factors associated with road accidents.

In response to the pressing need for comprehensive road safety solutions, we embark on a data analysis project focused on the RRCGB data for the years 2021 and 2022.

## Objective
Our objective is to develop a robust road accident dashboard that provides stakeholders with actionable insights derived from a meticulous examination of the available data.

### Tool used
- MS- Excel

## Business Requirements
Our client has articulated specific requirements for the road accident dashboard, driven by the imperative to enhance road safety measures. The primary Key Performance Indicator (KPI) is the total number of casualties resulting from accidents. Additionally, the client seeks insights into various aspects of road accidents, including:

**1. Total casualties and their distribution by accident severity:** Understanding the severity of accidents is crucial for prioritizing interventions. We will analyze the distribution of casualties based on accident severity and identify the types of vehicles involved in accidents with the highest casualty rates.

**2. Secondary KPIs:**
- Total casualties categorized by vehicle type.
- Monthly trend analysis to compare casualties between the current and previous years, enabling the identification of seasonal variations or emerging trends.
- Distribution of casualties by road type to ascertain whether certain road configurations are more prone to accidents.
- Examination of casualties concerning road surface conditions, highlighting the impact of weather and infrastructure maintenance.
- Exploration of the relationship between casualties, geographical location, and light conditions, providing insights into the role of visibility in accident occurrence.

## Data Overview
The data utilized in this project originates from the Reported Road Casualties Great Britain (RRCGB), the official statistical publication of the UK Department for Transport (DfT) on traffic casualties and road safety data. For further details on the RRCGB, you can refer to the Wikipedia page here.

The dataset provided for analysis is in Excel (.xlsx) format and comprises 21 fields capturing various attributes related to road accidents. With a total of 307,974 rows, this dataset offers a comprehensive overview of road incidents during the years 2021 and 2022.

## Data Cleaning
Sorting the dataset to facilitate efficient analysis.
Verifying the integrity of the primary key, the Accident Index, and eliminating duplicate values.
Identifying and addressing null values to prevent data distortion and bias in our analysis
Rectifying inaccuracies such as spelling errors in the Accident Severity column, ensuring consistency in data representation.
The accident severity column had a spelling mistake. Some of the rows for fatal were spelt as fetal so using the find and replace, I replaced all the rows having “fetal” to ‘fatal”.

![image](https://github.com/Orie05/Road_Safety_Analysis/assets/149834782/2bd02cce-dfe8-46e1-9938-9ade6afe330c)

49 replacements were made

## Data Processing
In the data processing, we will be adding new columns that are helpful in answering the business question and clients requirement.

1. Extracting month name from accident date using the following formula
   
![image](https://github.com/Orie05/Road_Safety_Analysis/assets/149834782/0ebd5000-973c-4a5f-9331-145ab2b8d522)


2. We repeat the process to extract the year from accident date.
   
![image](https://github.com/Orie05/Road_Safety_Analysis/assets/149834782/a5dcc975-2ab1-489e-835a-c00b25c5cf81)


## Data Analysis and Visualizations
Here we analyze the dataset using pivot tables.

**1. Total casualties and their distribution by accident severity:**

![image](https://github.com/Orie05/Road_Safety_Analysis/assets/149834782/8e960d3c-0c5b-4eae-9922-63460adaf2b2)

Using the GETPIVOTDATA formula, we extract the values in a pivot table and express as a percentage of total.


**2. To identify the types of vehicles involved in accidents with the highest casualty rate.**

Create a pivot table showing vehicle type as row and number of casualties as values.

![image](https://github.com/Orie05/Road_Safety_Analysis/assets/149834782/a1845b15-027d-427c-b113-bb346f628cb2)


**3. Distribution by vehicle type**

![image](https://github.com/Orie05/Road_Safety_Analysis/assets/149834782/0023d282-0a9d-4305-a1fb-7afa1c871462)


Using the ‘calculated items’ options in the ‘fields, items and sets’ button, we consolidate into 6 categories

![image](https://github.com/Orie05/Road_Safety_Analysis/assets/149834782/227f6691-cff7-4627-8464-496f5a1456ee)


**4. Monthly trend analysis to compare casualties between the current and previous years.**

![image](https://github.com/Orie05/Road_Safety_Analysis/assets/149834782/e137c527-7ecd-453d-975b-97ac3189e4ba)


**5. Distribution of casualties by road type.**

![image](https://github.com/Orie05/Road_Safety_Analysis/assets/149834782/56e53bdd-b012-4bd1-ae2b-bae14eb781a3)


**6. Examination of casualties concerning road surface conditions.**

![image](https://github.com/Orie05/Road_Safety_Analysis/assets/149834782/52840cd2-d7ab-41b2-9748-2a447c3cd0de)


Regrouping into three categories

![image](https://github.com/Orie05/Road_Safety_Analysis/assets/149834782/239c3e8f-74ad-4479-baa4-d34852597985)


**7. Exploration of the relationship between casualties and light conditions.**

![image](https://github.com/Orie05/Road_Safety_Analysis/assets/149834782/6bd1e7af-f2ae-4400-85ac-c9e382a6a589)


**8. Distribution of casualties based on geographical location**

![image](https://github.com/Orie05/Road_Safety_Analysis/assets/149834782/cd060e9e-1c3b-47bf-bf43-89cfc4a7869c)


Inserting timelines and slicers to filter data and create a more interactive and user-friendly dashboard

![image](https://github.com/Orie05/Road_Safety_Analysis/assets/149834782/362a5ddc-0e69-4834-a8ff-b9192bffb66d)


![image](https://github.com/Orie05/Road_Safety_Analysis/assets/149834782/8c146d8f-b3ec-45bc-9733-9405ee32c4f4)



## INSIGHTS
- We’ve recorded a total of 417,883 casualties.
- The majority of casualties are classified as slight, accounting for 84.1% of the total. Serious casualties make up 14.2%, while fatal casualties are comparatively lower at 1.7%.
- Cars are the most involved vehicle type, contributing to nearly 80% of total casualties. Bikes and buses also have significant contributions, while other vehicle types make up the remaining proportion.
- In general, 2022 witnessed a decrease in casualties compared to 2021. Notably, February showed a similar number of casualties between the two years.
- Single carriageways appear to be the most common location for accidents, followed by double carriageways and roundabouts. Slip roads and one-way streets have relatively lower casualty counts.
- Accidents predominantly occur on dry road surfaces, with wet conditions being the next most common. Snow and ice contribute to a smaller proportion of accidents.
- Daylight conditions witness a higher number of casualties compared to dark conditions.
- Rural areas report a significant number of casualties, although urban areas have a higher overall count. This highlights the need for tailored interventions in both settings to address specific challenges.


## RECOMMENDATIONS
- Allocate resources to enhance emergency medical services to effectively respond to serious and fatal accidents, minimizing casualties.
- Introduce targeted safety campaigns aimed at car drivers to address their significant contribution to overall casualties.
- Implement seasonal road safety initiatives to address trends observed during high-casualty months, adapting strategies as per seasonal variations.
- Direct resources towards improving safety measures on single carriageways, which exhibit the highest casualty counts, to reduce accident rates.
- Invest in infrastructure maintenance and weather-responsive road management to mitigate accidents during adverse conditions, such as wet, snowy, or icy road surfaces.
- Analyze driver behavior patterns during daylight hours to identify common risky behaviors such as speeding, distracted driving, or aggressive maneuvers.
- Assess the impact of environmental conditions during daylight hours, such as glare from the sun, changing weather conditions, or increased traffic volume, on accident occurrence.
- Develop targeted road safety initiatives for urban areas to address the unique challenges of densely populated environments, focusing on pedestrian safety, traffic management, and infrastructure improvements.
- Strengthen enforcement of traffic regulations and promote public awareness campaigns to improve road user behavior and reduce the severity of accidents, emphasizing compliance with speed limits, seat belt usage, and avoiding distracted driving.


## DASHBOARD

![image](https://github.com/Orie05/Road_Safety_Analysis/assets/149834782/17c003d9-cd9c-47ec-b49f-48f37e71a54f)



