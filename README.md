# Navigating the Git Repository
![777x-hero_1280x720](https://github.com/alecs1523/Aviation_Data_Analysis/assets/48231231/c69d4120-e48f-4fbc-80c8-9a18597799ae)

## Overview
### This project analyzes historical aviation data from 1948-2022 with a focus on accident history. Aviation accidents can be contributed to many variables and the goal of this project is to identify ~3 critical data points that attribute the most to aviation accidents. A business evaluating which type of airplane to use for its business can use these findings to select the best investment for them.

## Business Problem
### A business is uncertain which type of airplane it should invest in. 

## Data Sources
### aviation_data.csv - main data source used for analysis
### us_state_codes.csv - codes for every US state

## Presentation Links
### PowerPoint: https://github.com/alecs1523/Aviation_Data_Analysis/blob/main/phase_1_aviation_analysis.pptx
### PDF: 


# Business Understanding
## Goal
### Identify the variables that make an airplane safe and provide business reccomendations based on this analysis. 

# Data Understanding
### Dataset Overview
#### Summary: The dataset contains records of aircraft crashes between 1948 - 2022. The data from 1948 -1982 is limited so we drop those data points to focus on the majority of the volume following 1982. Data points include the number of engines, seveirty of passenger injuries, severity of aircraft damage,and more.

### Important Data Columns:

Aircraft Make and Model: Information about the specific make and model of the aircraft involved in each incident.

Aircraft Damage: The severity of the damage to the aircraft

Severity of Injuries: A count for each incident on the number of uninjured, minor, serious, and fatal injuries.

Engine Type: The type of engine being used in the aircraft

Num of Engines: Thye # of engines on the aircraft.

### Dataframe Key Statistics

![image](https://github.com/alecs1523/Aviation_Data_Analysis/assets/48231231/f552e02d-0e8d-48ce-82e9-9c38b079ba52)


# Data Preparation
### Prepare data for analysis

The dataframe has 88889 rows and 31 columns. 

There are several columns missing values in more than 25% of rows which we will drop to ensure significant population of results. The columns we drop are ['Latitude', 'Longitude', 'Airport.Code', 'Airport.Name', 'Aircraft.Category', 'FAR.Description', 'Schedule', 'Air.carrier', 'Broad.phase.of.flight']

# Exploratory Data Analysis
Explore the impact different engine types have on plane safety
Visualize if there is a correlation between engine type and the severity of aircraft damage
![download](https://github.com/alecs1523/Aviation_Data_Analysis/assets/48231231/c01b59d4-dea3-4d3a-a506-e4b071b6e584)

Explore the impact different number of engines has on plane safety
Visualize if there is a correlation between number of engines and the severity of aircraft damage
![download](https://github.com/alecs1523/Aviation_Data_Analysis/assets/48231231/afdf1020-4552-402c-a6c2-dcd0f9edc8cb)

Explore the safest airplane maker and analyze different metrics such as the severity of aircraft damage and injuries

Visualize if there is a correlation between airplane manufacturer and the severity of aircraft damage
![download](https://github.com/alecs1523/Aviation_Data_Analysis/assets/48231231/17439219-3fe0-4836-ad15-bbd31d38c5cc)

# Dive Deeper Into Boeing
Analyze Boeing at a deeper level after identifying it as the safest manufacturer

![download](https://github.com/alecs1523/Aviation_Data_Analysis/assets/48231231/2972ec48-1d85-444a-8ef9-a38485d1f813)


# Conclusion
My recommendation is to look for Boeing made airplanes, specifically the 777 and 747 models, preferably with The Turbo Fan and Turbo Jet engine, and 3-4 engines.

This recommendation is supported by 4 key pieces of data found during analysis.
1. Boeing has the lowest percentage of destroyed aircrafts when compared to other Makes.
2. The 777 and 747 models have the lowest destroyed and substantial percentage compared to other Boeing models.
3. Turbo Fan and Jet engines have the lowest destroyed percentage damage
4. Planes with 3-4 engines have the lowest percentage of destroyed / substantial damage.


