# Analyzing Vehicle Theft in New Zealand

![theft](https://github.com/OjeabuluFaith/SQL_showroom/assets/67393979/087c8b14-0b68-47de-a854-c5e13008e6d9)


## Goal of project 
This project aims to support the New Zealand Police Department's efforts to enhance public awareness regarding the issue of motor vehicle theft. By providing crucial insights into the patterns and trends of vehicle theft, the initiative seeks to inform and educate the community, thereby contributing to the reduction of such crimes.

## Objective 
 - Determining the time frames during which vehicles are most susceptible to theft.
 - Identifying the types of vehicles that are most at risk of being stolen.
 - Pinpointing the locations where vehicle thefts are most likely to occur.
 

## About dataset 
This dataset encompasses geospatial, time-series, and government data, focusing on stolen vehicle details from the New Zealand Police Department. It is structured into three main tables: Location, Make_Details, and Stolen_Vehicle, each providing critical insights into vehicle theft incidents.

Key Features
Tables Included: Location (geographical data), Make_Details (vehicle make and model), and Stolen_Vehicle (comprehensive theft details).

Important Fields: Vehicle ID, type, make ID, model year, color, and theft region, facilitating an in-depth analysis of theft patterns.







### Steps followed 

The analysis of vehicle theft patterns in New Zealand was meticulously carried out using MySQL, focusing on extracting, grouping, and joining data to meet the project's objectives.

- Step 1: To determine the frequency of car thefts by day of the week and month, we utilized the SELECT and GROUP BY statements on the stolen_vehicles table. This step involved calculating the total number of vehicles stolen on each day and month.

![day_of the week](https://github.com/OjeabuluFaith/SQL_showroom/assets/67393979/a0c4ceed-4170-4b5b-8efc-e893b6be27dd)



- Step 2: To identify the types of vehicles most and least susceptible to theft, we analyzed the vehicle_type field. By sorting the amount of each type stolen in descending order, we pinpointed the vehicle types most and least targeted by thieves.


![vehichle type stolen more](https://github.com/OjeabuluFaith/SQL_showroom/assets/67393979/6f230659-cef0-463e-a30f-2483d7908df8)

![vehichle(object 2)](https://github.com/OjeabuluFaith/SQL_showroom/assets/67393979/90a3ddd4-351b-425b-906a-4c91ec9fe0f5)




- Step 3: The final objective focused on identifying theft hotspots across different New Zealand cities. By performing a LEFT JOIN between the location and stolen_vehicles tables, we extracted and grouped data by region, population, and the number of vehicles stolen, thereby revealing regional theft patterns.

![regions](https://github.com/OjeabuluFaith/SQL_showroom/assets/67393979/b378bdc0-6d40-4b0c-b365-c14775c8e5c7)




## Results and Visualization
The outcomes of the analysis were exported to CSV files for visualization:

- A bar chart illustrated the distribution of car thefts across different days of the week, providing insights into when thefts were most likely to occur.

![bar chart](https://github.com/OjeabuluFaith/SQL_showroom/assets/67393979/b331dfc6-bec3-4772-9c87-e67559def47f)


- A heat map was employed to visualize the relationship between vehicle type, color, and theft frequency, offering a clear view of the most vulnerable vehicles.

![heatmap](https://github.com/OjeabuluFaith/SQL_showroom/assets/67393979/7eda95bc-0aef-4fb9-8504-c503defafd7f)

- For regional analysis, a map and bubble visualization highlighted areas with the highest and lowest incidence of vehicle theft, aiding in the identification of critical theft zones.

![bubble chart](https://github.com/OjeabuluFaith/SQL_showroom/assets/67393979/51b1c52f-24c3-44e8-8825-444dea881adb)


![map](https://github.com/OjeabuluFaith/SQL_showroom/assets/67393979/da6879c2-c233-45a6-ba75-391a1090e3c9)

 



 


# Insights
- Total Vehicle Thefts: The analysis revealed a total of 4,553 vehicles were stolen across the country.

- Most Frequently Stolen Vehicles: The types of vehicles most targeted by thieves include station wagons, saloons, hatchbacks, trailers, and utility vehicles. Conversely, special purpose vehicles, articulated trucks, and trail bikes were among the least frequently stolen.

- Regional Theft Rates: Auckland emerged as the region with the highest number of stolen vehicles, totaling 1,638 incidents. This figure is significant, considering Auckland's population of 1,695,200 and a density of 343.09 individuals per square kilometer. In stark contrast, the Southland region reported the lowest theft rate, with only 26 vehicles stolen, correlating with its smaller population of 102,400 and a density of 3.28.

- Vehicle Age: The average age of stolen vehicles was found to be 19 years, indicating a particular vulnerability of older vehicles to theft.

- Temporal Patterns: March witnessed the highest number of vehicle thefts, with a total of 1,053 incidents, followed by February, which saw 763 thefts. This temporal distribution provides insights into potential periods of increased theft risk.



# Recommendation

Based on the insights gleaned from the data, I recommend the following actions:

- Enhanced Security Measures: Implementing stronger security measures for the most frequently stolen vehicle types and in regions with high theft rates, particularly Auckland.

- Public Awareness Campaigns: Launching awareness campaigns focused on the months with the highest theft rates, encouraging vehicle owners to adopt preventive measures.

- Older Vehicle Protection: Special attention should be given to the security of older vehicles, which are shown to be more susceptible to theft.
