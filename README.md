# Urban Cup 2023

## Dear Participants,
Welcome to Urban Cup 2023 of the first Research Summit on Urban Science and Human Dynamics! We sincerely invite you and your team to join the fascinating journey towards data-driven urban science for sustainability and social good! With fine-grained data on urban mobility, local infrastructure, land use, gas emission as well as poverty, health insurance, education attainment, etc., we welcome you to submit an original and publicly understandable impression of urban phenomena, patterns, or connections concerning urban sustainability and social good. The impression should be aesthetically, scientifically, and accurately visualized based on your data analysis. **Two or more** forms of the provided data should be used, and additional information (e.g., Internet activities) may but need not be linked to. Please also make sure to submit the source codes that guide you to your amazing discoveries.

Please summarize the impression in a **one-page slide** and format your submission as [this template](Submission_Format.pptx). Each team should consist of **no more than 3 people**, with **at least one** team member present at the conference venue to **present the impression**. Please email all files to **rsushd2023@163.com by August 5th @ 8am (Beijing time, UTC/GMT+08:00)** to complete the submission. Late submissions will not be considered. 

Exemplar ideas of the impressions can be found [here](src/Exemplar_Ideas.md).

## Datasets
We provide **6 city-scale datasets** collected from the largest U.S. cities and **1 sub-city scale multisourced dataset** collected from 1039 middle layer super output areas (MSOAs) of 29 England cities, which are briefly described as follows: 

### 1. U.S. mobility dataset
This dataset is extracted from SafeGraph. It details the monthly population movement between CBGs within the 10 largest cities in the United States from 2018.1 to 2022.4. The movements were aggregated from anonymized mobile devices. Please click [here](Data_Description/Mobility/Readme.md) for more details about the dataset.

### 2. U.S. carbon emission dataset
This dataset is collected from Open-source Data Inventory for Anthropogenic CO2 (ODIAC). It records the CO2 emission within the 10 largest cities in the United States between 2018 and 2021. The data provides monthly CO2 emissions from fossil fuel combustion, cement production and gas flaring on a 1x1 km spatial resolution. Please click [here](Data_Description/Carbon/Readme.md) for more details about the dataset.

### 3. U.S. air pollution dataset
This dataset is derived from the Environmental Protection Agency of the United States. It is collected from air quality monitors and consists of the daily O3, SO2, NO2, CO, PM2.5, and PM10 information across the United States between 2018 and 2021. Please click [here](Data_Description/Air_Pollution/Readme.md) for more details about the dataset.

### 4. U.S. population characteristic dataset
This dataset is obtained from American Community Survey (ACS), Earth Observation Group and OpenStreetMap. It provides both CBG-level and city-level poverty, health insurance, education, income Gini & light Gini, and built environment & racial segregation data from 2014 to 2023 across the 10 largest cities in the United States. Please click [here](Data_Description/Population/Readme.md) for more details about the dataset.

### 5. U.S. visual semantics dataset
This dataset provides semantic attributes processed from satellite remote sensing data. It depicts both CBG-level and city-level urban infrastructural information from 2014 to 2023 across the 10 largest cities in the United States. Please click [here](Data_Description/Visual_Semantics/Readme.md) for more details about the dataset.

### 6. U.S. basic geographical information dataset
This dataset consists of basic geographical information of CBGs across the 10 largest cities in the United States between 2014 and 2021. It records the city, area, population, centroid, and boundary of the CBGs within each year. Please click [here](Data_Description/Basic_Geographic_Info/Readme.md) for more details about the dataset.

The data entries of the above mentioned datasets are summarized as below:

![Image text](Data_Description/Data.png)

### 7. England evironment and health datasets
This is a fine-grained and multi-sourced environment and health dataset collected from cities in England. It records the health outcomes of citizens covering physical health (COVID-19 cases, asthma medication expenditure, etc.), mental health (psychological medication expenditure), and life expectancy estimations. It presents the corresponding environmental determinants from four perspectives, including basic statistics (population, area, etc.), behavioural environment (availability of tobacco, health-care services, etc.), built environment (road density, street view features, etc.), and natural environment (air quality, temperature, etc.). To reveal regional differences, this dataset extracts and integrates massive environment and health indicators from heterogeneous sources into two unified spatial scales, i.e., at the middle layer super output area (MSOA) and the city level, via big data processing and deep learning techniques.

A comprehensive data table that contains all the subsections is also provided, which is organized into a long table with columns as follows:
| Column Name | Description | Example |
| ------ | -----------|-----------|
| TopCategory| The top category of the dataset.| HealthOutcome, EnvironmentalDeterminants|
| SecondCategory |The second category of the dataset.| PhysicalHealth, MentalHealth, LifeExpectancy, NaturalEnvironment, BehaviourEnvironment, BuiltEnvironment, BasicStatistics|
| ThirdCategory | The third category of the dataset.| DementiaExpenditure, Weather, TobaccoAvailability, RoadDensity, Population |
| CityCode | Exclusive ID for each city. | J01000007|
| CityName | Name of the city. | Birmingham|
| MSOACode | Exclusive ID for each MSOA.| E02001834|
| MSOAName | Name of the MSOA. |Birmingham 008 |
| Time | Time of the data record. For those without timestamps, `None` is filled to this column.| 2019-01-01
| Key | Specifications of the record, such as  `Mean` for `HousePrice` and `Female` for `LifeExpectancy` |  Mean, Female, PM2.5 |
| Value | Value of the data record.| |
