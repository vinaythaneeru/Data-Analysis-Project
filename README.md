# Data-Analysis-Project
Collected used car data via web scraping, cleaned and analyzed it, and visualized key trends to identify factors affecting prices, helping buyers and sellers make informed decisions.
# Used Car Price Analysis

A comprehensive data analysis project that scrapes, cleans, and analyzes used car pricing data to identify trends and key factors influencing resale values.

## Project Overview

This project demonstrates a complete data science workflow—from web scraping to exploratory data analysis (EDA). We collected used car data from **CarDekho** and performed in-depth analysis to understand pricing patterns across different car attributes.

**Key Findings:**
- Most used cars are 3–10 years old  
- Diesel cars maintain higher resale prices on average  
- Transmission type and ownership history strongly influence price  
- Newer cars with lower kilometers command premium prices
- 
## Workflow

### 1. **Web Scraping**
- Collected raw car data from CarDekho using **BeautifulSoup**  
- Extracted: car name, year, price, fuel type, transmission, location, kilometers driven  
- Handled inconsistent website formats using Regular Expressions  
- Output: Raw CSV file for further processing  

### 2. **Data Cleaning**
- Removed duplicate and missing entries  
- Applied Regular Expressions to clean text fields and remove special characters  
- Standardized data types (Year, Kilometers, Price)  
- Renamed and reorganized columns for consistency  

### 3. **Data Manipulation**
- Extracted car brand from name field  
- Created new feature: **Car Age** = Current Year – Year of Manufacture  
- Filtered data for active sellers and valid prices  
- Grouped by brand, fuel type, and transmission  
- Aggregated statistics for comparison  

### 4. **Univariate Analysis**
- Analyzed individual variable distributions  
- Studied price segments and age distribution  
- Calculated mean, median, mode, and detected outliers  
- Fuel type distribution: Diesel & Petrol dominate  

### 5. **Bivariate Analysis**
- **Year vs Price:** Clear depreciation trend observed  
- **Fuel Type vs Price:** Diesel cars priced 10–15% higher  
- **Transmission vs Price:** Automatic cars command premium  
- **Ownership & Kilometers:** Strong inverse correlation with price  
- **Location-based patterns:** Price variation across regions  

### 6. **Exploratory Data Analysis (EDA)**
- Visualized distributions using histograms and boxplots  
- Correlation analysis between key features  
- Identified outliers and data inconsistencies  
- City-wise average price trends  

## Tech Stack

- **Python 3**  
- **Web Scraping:** BeautifulSoup, requests  
- **Data Processing:** Pandas, NumPy  
- **Data Cleaning:** Regular Expressions (re)  
- **Visualization:** Matplotlib, Seaborn  
- **Environment:** Jupyter Notebook  
 

## Key Insights

✅ **Price Depreciation:** Older cars lose value exponentially  
✅ **Fuel Efficiency Factor:** Diesel preferred in Indian market  
✅ **First Owner Premium:** First-owner vehicles retain 20–25% higher value  
✅ **Mileage Impact:** Every 100,000 km decrease = ~₹1–2 lakhs higher price  
✅ **Brand Reliability:** Popular brands command 15% higher average price  

## Challenges & Learnings

- **Web Scraping:** Handled dynamic website structures and anti-scraping measures  
- **Data Quality:** Dealt with missing values, inconsistent formats, and outliers  
- **Regex Complexity:** Applied advanced pattern matching for text cleaning  
- **Real-world Data:** Discovered importance of exploratory analysis before modeling  
- **Performance:** Optimized processing for 10,000+ records efficiently 
