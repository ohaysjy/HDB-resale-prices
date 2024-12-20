## HDB Resale Prices Predictive Modelling by using Linear Regression to accurately estimate competitive pricing for HDB resale flats for both buyers and sellers 

![HDB_News](/images/HDB_News.png) <br>
![HDB_History](/images/HDB_History.png) <br>

Over the years, HDB resale prices have been a hot topic among many Singaporeans. With million-dollar flats becoming increasingly common, along with fluctuations in the resale market, HDB owners face challenges in determining the optimal value for buying or selling their flats. <br>

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
