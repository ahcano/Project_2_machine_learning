# **Project Title**: GDP Growth Predicted by Machine Learning 
 
**Project Overview**: The objective of this project is to predict the Canada GDP Growth by applying Machine Learning algorithms to analyze relationships between the consumer price index and variables such as CDN TSX index, Prime Rate, Home Ownership Rate, GDP Growth and CDN/USD exchange rate.

# Introduction

Machine learning is a programming approach for designing applications that learn from their inputs and make adjustments based on their outputs. With that in mind, the problematic was to find a business problem to solve by applying Machine Learning. However, sourcing data posed a "chicken and egg" problem. After one of the team members found sample data of Consumer Price Index (CPI) - a relevant metric in the current socioeconomic environment, the team decided to embark on defining what to predict.

**GDP growth rate in Canada with actual historical data from 2005 to 2023.**
<p align="center">
    <img width="464" alt="Screenshot 2023-12-07 163758" src="https://github.com/ahcano/Project_2_machine_learning/assets/141194281/3bfd76be-f676-47da-9fb5-7de44285de76">
<p>

These images show GDP Growth in blue. It can be deducted that the COVID pandemic lockdown from the year 2020 introduced a spike of unemployment rate, historically shown in orange; while the GDP had a considerable decrease.
<p align="center">
<img width="447" alt="Screenshot 2023-12-07 175011" src="https://github.com/ahcano/Project_2_machine_learning/assets/141194281/fa72cfdd-0b89-4b6c-8e97-85ee053d8bc4">
<p>
This observation was one of the key motivators for the Fintech team to analyze other economic parameters and how their performance correlates, using Machine Learning algorithms to make a prediction of the GDP trend over the next few years. 
With the current economy struggle being a current "hot" topic of interest among industry analysts and the general population alike, we believe that this project promises to provide an interesting insight backed up by tangible facts, as well as a learning journey for the team participants. 

    
# Data Definitions and Sources

All source data was consolidated in **Starter_Data.csv** file and read into the Python dataframe **ohlcv_df**; the first five samples are shown below.
<p align="center">
<img width="765" alt="Screenshot 2023-12-06 180408" src="https://github.com/ahcano/Project_2_machine_learning/assets/141194281/102c12e8-f6dc-4cfa-ab1e-2d7608c04a7c">
<p>
    
* **Consumer Price Index (CPI)** is an economic measure of the monthly change in average goods and services prices paid by household consumers. 
    * The CPI is used as an indicator of inflation and is labeled as **price_indextor** in the dataframe. 
    * For this projects purpose, the Toronto CPI was used as the Canadian representative sample.
    * Data source:  Nasir

* **Price Index Change** 
    * Data source: **price_indextor** dataframe column.?????????????????
    * Calculated as a monthly decimal percentage change.
      
* **Inflation Rate**
    * According to _Wikipedia_, inflation is a general increase of prices of goods and services in an economy.
    * Inflation is usually measured using the CPI.
    * data is labelled as **inflation_rate** on the dataframe.
    * Data source:  
      
* **Canadian Prime Rate**
    * Annual interest rate used by Canadian banks for variable loans and lines of credit, including variable-rate mortgages.
    * The prime rate is primarily influenced by the policy interest rate set by the Bank of Canada.
    * data is labelled as **canadian_prime_rate** on the dataframe.
    * Data source:  Nasir

* **S&P/TSX Index**
    * According to _Wikipedia_, this Canadian index represents roughly 70% of the total market capitalization on the Toronto Stock Exchange (TSX).
    * As of September, 2021 the S&P/TSX composite index comprises 237 of the 3,451 companies listed on the TSX.
    * Securities are generally eligible for inclusion in the composite index by satisfying regulations of market capitalization, liquidity and incorporation under Canadian laws.
    * data is labelled as **cnd_tsx_indx** on the dataframe.
    * Data source:  Ryan

* **Unemployment rate**
    * This measure is used to track the number or people above 15 years of age that are available for work but are not paid by employment. 
    * data is labelled as **unemployment_rate** on the dataframe.
    * Data source:  Andrew

* **Home ownership rate**
    * Data source:  Ryan

* **GDP Growth** . Gross domestic product (GDP) is a monetary measure of the market value of all final goods and services produced in a specific period by a country. In this case, Canada.
    * GDP growth is represented as a decimal percentage rate, labeled **GDP_growth** in the dataframe.
    * If positive, the number indicates growth compared to the previous month.
    * A negative rate means there was a decrease relative to the prior month.
    * data is labelled as **GDP_growth** on the dataframe.
    * Data source:  Andrew

* **Canadian - US Dollar Exchange Rate**
  * Currencies are traded through BUY/SELL transactions in Foreign Exchange (FOREX) markets globally.
  * Labelled **CND_USD_exchange** in the dataframe.
  * Data source: https://www.ofx.com/en-ca/forex-news/historical-exchange-rates/monthly-average-rates/ 

# Usage 

This project is for information purposes only and is not intended to be used as a base for any high risk investments. The predictions offer only a perspective created artificially using python code ;-)

# Summary of the Analysis

Since the GDP values are continuous, Supervised Learning Regression models were selected for the machine learning prediction approach and variables. 
* The first model was a **neural network**. 
* The second one, **linear regression**.

Supervised learning involves three steps for predicting an output: preparing the input data, fitting the model and building the model.
As an input to both models, the data is split into **X (features)** and **y (target)** variables. Where **y** is GDP_growth, and **X** is all other data labels.

# Results

**GDP growth rate prediction 2023---??**
_INSERT IMAGE HERE_

## Data clean up involved removal of blank spaces:
<p align="center">
 <img width="419" alt="Screenshot 2023-12-06 181022" src="https://github.com/ahcano/Project_2_machine_learning/assets/141194281/463306da-6a26-4048-adeb-aa95f692d7c6">
<p>
## Data was normalized using the standard scaler command
<p align="center">
 <img width="382" alt="Screenshot 2023-12-06 181209" src="https://github.com/ahcano/Project_2_machine_learning/assets/141194281/845d165f-6e3a-4e1b-938e-8b79e0b120ac">
<p>

# Fintech Analysis and Development
* Ryan Judd
* Andrew Gopan
* Nasir Farah
* Ana Cano

