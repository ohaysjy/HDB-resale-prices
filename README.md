# HDB Resale Prices Predictive Modelling

## Introduction

![HDB_History](/images/HDB_History.png) <br>

Over the years, HDB resale prices have become a hot topic among many Singaporeans. As million-dollar flats become increasingly common, combined with fluctuations and competitive pricing in the resale market, both homeowners and tenants find that mortgage payments or monthly rent can consume a significant portion of their income. Therefore, accurately determining the optimal transacted value is invaluable for buyers and sellers, providing insights into the current resale market. <br> 

The goal of this data-driven tool is to:  
- Provide competitive pricing advice for clients looking to buy or sell their HDB resale flats.  
- Accurately estimate the resale values of HDB flats based on different types and locations.  

## Problem Statement
> HDB Resale Prices Predictive Modelling by using Linear Regression to accurately estimate competitive pricing for HDB resale flats for both buyers and sellers

## Datasets 

Source: https://www.kaggle.com/competitions/dsi-sg-project-2-regression-challenge-hdb-price/data <br>

There are three files: <br>
- train_data.csv: 78 Columns by 150,634 Rows (January 2012 to April 2021)
- test_data.csv: 78 Columns by 16,737 Rows (March 2012 to April 2021)


## Data Cleaning 
1. Replacing missing values with '0' for 'mall within 500m, 1km, and 2km' and also for 'hawker within 500m, 1km, and 2km' <br>
2. Remove 829 data for 'mall nearest distance' <br>
3. Checked for duplicates <br>
4. Convert date columns to datetime format <br>

## Data Exploration 
Let’s examine how the trends in HDB resale prices have evolved over the years based on various factors. <br>

![HDB_Distribution_Price](/images/HDB_Dist_Price.png) <br>

Based on the physical factors of HDB flats: <br>
![HDB_Floor_Area](/images/HDB_Floor_Area.png) <br>
![HDB_Flat_Type](/images/HDB_Flat_Type.png) <br>
![HDB_Storey](/images/HDB_Storey.png) <br>

Based on the different regions of HDB flats: <br>
![HDB_Regions](/images/HDB_Regions.png) <br>
![HDB_Regions_One](/images/HDB_Regions_1.png) <br>
![HDB_Regions_Two](/images/HDB_Regions_2.png) <br>

Based on the Supermalls in Singapore: <br>
![HDB_Supermall](/images/HDB_Supermall.png) <br>

Tableau HDB Resale Price Interactive Dashboard: <br>
![HDB_Interactive_Dashboard](/images/HDB_Interactive_Dashboard.png) <br>

A) First Predictive Modelling using **'town', 'floor area', 'lease commence date', 'resale price', 'transaction year and month', 'distance to nearest mall', 'distance to nearest hawker', and 'distance to nearest MRT'** as the first features. <br> 

![HDB_Pred_One](/images/HDB_Pred_One.png) <br>

<u>Conclusion: </u> <br>
Using the features detailed above, the Room Mean Square Error (RMSE) is $60,772.38. This indicates that the model can predict the resale value of the HDB flat with a variance of $60,772.38 from the actual price. Additionally, an R² value of 0.82 suggests that the model effectively explains 82% of the variation in the resale value of the HDB flats. <br> 

B) Second Predictive Modelling using **'town', 'floor area', 'lease commence date', 'resale price', 'transaction year and month', 'distance to nearest mall', 'distance to nearest hawker', 'distance to nearest MRT' and 'HDB storey'** as the second features. <br> 

![HDB_Pred_Two](/images/HDB_Pred_Two.png) <br>

<u>Conclusion: </u> <br>
Using the features detailed above, the Room Mean Square Error (RMSE) have improved to a value of $55,431.29. This indicates that the model can predict the resale value of the HDB flat with a variance of $55,431.29 from the actual price. Additionally, an R² value of 0.85 suggests that the model effectively explains 85% of the variation in the resale value of the HDB flats. <br> 
