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
### Outcome [Apple's greenhouse gas emissions dashboard.pdf](https://github.com/user-attachments/files/22703956/Apple.s.greenhouse.gas.emissions.dashboard.pdf)
-	 (1) Apple decreased emission (without offset) between 2015 and 2022 from 38.38M tCO2e to 20.60M tCO2e. It means -46.32% decrease at all and -8.50% CAGR (Compound Annual Growth Rate).
-	 (2) While emission decreased (-8,50% CAGR) between 2015 and 2022, revenue (+7.76% CAGR) and market cap (+23.14% CAGR) increased in the same period (decoupling).
-	 (3) While manufacturing, product use, business travel, employee commute and and-of-life processing had the highest impact to the decrease and performed best, product transportation increased seriously (+46.15%).
-	 (4) Considering fact emission CAGR between 2015 and 2022 (-8.50%) and required emission CAGR between 2023 and 2030 (-9.11%) with some actions Apple can reach their target emission. Along with this they need provide 1.20M tCO2 removal between 2023 and 2030, which can be very challenging and required a strict and consistent strategy from the company.

![Image](https://github.com/user-attachments/assets/1d3268fa-6269-40c6-9720-d58e5c2d5252)
### Methods and steps
#### Loading, transforming, cleaning and exporting data with Python
Important step during data preparation is outlier detection. As the data in our case doesn’t follow normal distribution IQR (interquartile range) method was used, which is a robust measure because it is not affected too much by extreme outlier values. Finally outliers were also considered as valuable data, as in case of GHG emissions they are not mistakes or wrong detected values.
![Image](https://github.com/user-attachments/assets/05543c77-50c6-435d-9b6f-ba163595cad9)
![Image](https://github.com/user-attachments/assets/d20e9bfa-d1ca-4cf7-a57c-c2c78e6b0391)
![Image](https://github.com/user-attachments/assets/44af4532-6cea-4ef2-b6ff-0263c8a08e4d)
![Image](https://github.com/user-attachments/assets/be745bea-6613-4c56-841e-d21a1e939bc0)
![Image](https://github.com/user-attachments/assets/dc8d1420-a2b2-495c-8305-9d95184ec82b)
![Image](https://github.com/user-attachments/assets/b4acbc5f-cc10-428c-8d7b-0b6ad3ff6a16)
#### Importing, analyzing and visualizing data in PowerBI
Analyzing data with using DAX measures in order to use them anywhere in the report, referenced by other DAX measures and provide more complex calculations. Some of the most important measures:
![Image](https://github.com/user-attachments/assets/a6ebfded-ca3f-487f-978a-47f22f6c7937)
![Image](https://github.com/user-attachments/assets/221c1b99-5b08-4ff2-a49c-a634e4bfc82b)
![Image](https://github.com/user-attachments/assets/def9e747-70aa-4825-bcd8-462f107bc6c7)
![Image](https://github.com/user-attachments/assets/a6ecbc64-6fdd-416b-8b2b-632332174a6a)
