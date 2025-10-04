## Apple’s greenhouse gas emissions project - way to net zero emission until 2030
### Starting point
Apple Inc. set the goal to reach a high level of sustainability through net zero emission until 2030. They planned to reduce carbon emission from 38.4M tCO2e (2015 level) with 75% and descend to 9.6M tCO2e. The rest 25% is planned to cover by carbon offsets.
### Goal
The aim of the analysis to answer 4 important questions:
-	 (1) How much has Apple reduced emissions from 2015 to 2022?
-	 (2) How does this trend compare to revenue & market cap trend in the same period?	 
-	 (3) Which areas have seen the most improvement? What about the least?
-	 (4) Is Apple on track to meet their 2030 goal of net zero emissions?
### Data set
The CSV files contain data between 2015 and 2022 for each years about the followings:
-	gross carbon emissions and carbon removals/offset (tCO2e)
-	categories (corporate emission, product life cycle emission) and detailed areas
-	revenue, market capitalization and number of employees
### Outcome
-	 (1) Apple decreased emission (without offset) between 2015 and 2022 from 38.38M tCO2e to 20.60M tCO2e. It means -46.32% decrease at all and -8.50% CAGR (Compound Annual Growth Rate).
-	 (2) While emission decreased (-8,50% CAGR) between 2015 and 2022, revenue (+7.76% CAGR) and market cap (+23.14% CAGR) increased in the same period (decoupling).
-	 (3) While manufacturing, product use, business travel, employee commute and and-of-life processing had the highest impact to the decrease and performed best, product transportation increased seriously (+46.15%).
-	 (4) Considering fact emission CAGR between 2015 and 2022 (-8.50%) and required emission CAGR between 2023 and 2030 (-9.11%) with some actions Apple can reach their target emission. Along with this they need provide 1.20M tCO2 removal between 2023 and 2030, which can be very challenging and required a strict and consistent strategy from the company.
[Apple_project.pdf](https://github.com/user-attachments/files/22703903/Apple_project.pdf)
### Methods and steps
#### Loading, transforming, cleaning and exporting data with Python
Important step during data preparation is outlier detection. As the data in our case doesn’t follow normal distribution IQR (interquartile range) method was used, which is a robust measure because it is not affected too much by extreme outlier values. Finally outliers were also considered as valuable data, as in case of GHG emissions they are not mistakes or wrong detected values.
#### Importing, analyzing and visualizing data in PowerBI
Analyzing data with using DAX measures in order to use them anywhere in the report, referenced by other DAX measures and provide more complex calculations. Some of the most important measures:
