# Navigating the Git Repository

## Data Sources
### aviation_data.csv - main data source used for analysis
### us_state_codes.csv - codes for every US state

## Presentation Links
### PowerPoint: https://github.com/alecs1523/Aviation_Data_Analysis/blob/main/phase_1_aviation_analysis.pptx
### PDF: 

![Uploading image.png…]()

# Business Understanding
## Goal
### Identify the variables that make an airplane safe and provide business reccomendations based on this analysis. 

# Data Understanding
### Dataset Overview
#### Summary: The dataset contains records of aircraft crashes between 1948 - 2022. The data from 1948 -1982 is limited so we drop those data points to focus on the majority of the volume following 1982. Data points include the number of engines, seveirty of passenger injuries, severity of aircraft damage,and more.

### Important Data Columns:

#### Aircraft Make and Model: Information about the specific make and model of the aircraft involved in each incident.

#### Aircraft Damage: The severity of the damage to the aircraft

#### Severity of Injuries: A count for each incident on the number of uninjured, minor, serious, and fatal injuries.

#### Engine Type: The type of engine being used in the aircraft

#### Num of Engines: Thye # of engines on the aircraft.

# Data Preparation
### Prepare data for analysis

The dataframe has 88889 rows and 31 columns. 

There are several columns missing values in more than 25% of rows which we will drop to ensure significant population of results. The columns we drop are ['Latitude', 'Longitude', 'Airport.Code', 'Airport.Name', 'Aircraft.Category', 'FAR.Description', 'Schedule', 'Air.carrier', 'Broad.phase.of.flight']



# Exploratory Data Analysis
#### Explore the safest airplane maker and analyze different metrics such as the severity of aircraft damage and injuries

#### Visualize if there is a correlation between airplane manufacturer and severity of aircraft damage

top_10_damage_by_make_percentage.plot(kind='bar',stacked=True)
plt.legend(bbox_to_anchor=(1.29,1),loc='upper right',borderaxespad=0)

plt.show()

# Dive Deeper Into Boeing
#### Analyze Boeing at a deeper level after identifying it as the safest manufacturer

# Conclusion
#### 1. Boeing is the safest aircraft manufacturer 2. The 777 is the safest model based on the severity of damage during accidents 3. Overall, aircraft accidents have been on the decline for many years

## Recommendations
#### My recommendation is to exclusively use Boeing airplanes and specifically the 777, 737, and 737-200 models
