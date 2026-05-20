
# MIS-311
Introduction to Business Analytics

*Project Overview 
This project focuses on cleaning, preparing, and analyzing an Electric Vehicle (EV) registration dataset to uncover meaningful business insights regarding market share and production trends.

# Electric Vehical Data Analysis 

## 1. Data Overview 

This tabular dataset contains registration information for eco-friendly vehicles—specifically Electric Vehicles (EVs) and Plug-in Hybrid Electric Vehicles (PHEVs)—in Washington State, USA

* Data Scale:

Total Rows: 143 rows (consisting of 1 header row and 142 detailed vehicle data records).

Total Columns: 5 original data columns displayed on the interface.

* Key Attributes (Features):

Vehicle Identification Number (VIN): A unique identifier for each vehicle (partially masked for privacy and data security).

City: The registered city of the vehicle (e.g., Seattle, Olympia, Bremerton, Poulsbo, etc.).

Postal Code: The ZIP/Postal code of the managing jurisdiction.

Model Year: The production year of the vehicle (ranging from older 2011 models to the latest 2025 releases).

Make & Model: A combined column containing both the vehicle Manufacturer (Make) and the specific designation (Model).

## 2. Data Cleaning 

Handling Duplicates via VIN Alignment: Since the Vehicle Identification Number (VIN) must be a unique identifier for each vehicle, a deduplication process was performed. All duplicate rows based on the VIN column were successfully removed to prevent data inflation.

Text Standardization (TRIM & PROPER): * Applied the TRIM function across the dataset to eliminate any leading, trailing, or inconsistent webpage/input whitespaces.

Applied the PROPER function specifically to the Make and Model columns to standardize capitalization (e.g., converting inconsistent text into clean title case), ensuring seamless grouping and filtering.

Data Type Formatting (Float to Integer): The Model Year column was converted from a float data type (e.g., 2018.0) to a clean integer format (2018) to accurately reflect chronological calendar years.

Missing Data Treatment (Missing Values): A thorough check revealed a few missing values (blank cells) within certain fields. However, because these missing data points accounted for an insignificant percentage of the total dataset, they were intentionally left as-is to preserve the remaining valid information without biasing the overall sample size.

## 3. Key Insinght 
 * Insight 1:
  
   We used a Pivot Table to quickly count the vehicles by brand and calculate their market share. From this table, we selected the Top 5 market leaders to see who is dominating the market and how new companies should respond.
   
   <img width="348" height="135" alt="11" src="https://github.com/user-attachments/assets/ba2e2feb-e18b-46d9-9ebc-f39ef5266399" />

   The Big Two: Tesla (47%) and Nissan (26%) are the clear kings of this market. Together, they own over 73% of the total market share.

   <img width="490" height="280" alt="EV registration distribution " src="https://github.com/user-attachments/assets/593a9052-83d5-43ac-a8bb-b9e5a68c144c" />


Advice for New Brands: The market is very crowded at the top.

Do not fight Tesla directly: Tesla is too strong with Model 3 and Model Y. Fighting them head-on in these segments is very risky.

Find a different path: New or smaller brands (like Hyundai, BYD, or startups) need to avoid Tesla's territory. Instead, they should focus on gaps that Tesla misses, such as cheaper budget EVs, electric trucks, or commercial delivery vans.

  


 * Insight 2  

