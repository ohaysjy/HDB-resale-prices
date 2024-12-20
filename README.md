## HDB Resale Prices Predictive Modelling by using Linear Regression to accurately estimate competitive pricing for HDB resale flats for both buyers and sellers 

![HDB_News](/HDB_News.png) <br>
![HDB_History](/HDB_History.png) <br>

Over the years, HDB resale prices have been a hot topic among many Singaporeans. With million-dollar flats becoming increasingly common, along with fluctuations in the resale market, HDB owners face challenges in determining the optimal value for buying or selling their flats. <br>

Let’s examine how the trends in HDB resale prices have evolved over the years based on various factors. <br>

![HDB_Distribution_Price](/HDB_Dist_Price.png) <br>

Based on the physical factors of HDB flats: <br>
![HDB_Floor_Area](/HDB_Floor_Area.png) <br>
![HDB_Flat_Type](/HDB_Flat_Type.png) <br>
![HDB_Storey](/HDB_Storey.png) <br>

Based on the different regions of HDB flats: <br>
![HDB_Regions](/HDB_Regions.png) <br>
![HDB_Regions_One](/HDB_Regions_1.png) <br>
![HDB_Regions_Two](/HDB_Regions_2.png) <br>

Based on the Supermalls in Singapore: <br>
![HDB_Supermall](/HDB_Supermall.png) <br>

Tableau HDB Resale Price Interactive Dashboard: <br>
![HDB_Interactive_Dashboard](/HDB_Interactive_Dashboard.png) <br>

A) First Predictive Modelling using **'town', 'floor area', 'lease commence date', 'resale price', 'transaction year and month', 'distance to nearest mall', 'distance to nearest hawker', and 'distance to nearest MRT'** as the first features. <br> 

![HDB_Pred_One](/HDB_Pred_One.png) <br>

<u>Conclusion: </u> <br>
Using the features detailed above, the Room Mean Square Error (RMSE) is $60,772.38. This indicates that the model can predict the resale value of the HDB flat with a variance of $60,772.38 from the actual price. Additionally, an R² value of 0.82 suggests that the model effectively explains 82% of the variation in the resale value of the HDB flats. <br> 

B) Second Predictive Modelling using **'town', 'floor area', 'lease commence date', 'resale price', 'transaction year and month', 'distance to nearest mall', 'distance to nearest hawker', 'distance to nearest MRT' and 'HDB storey'** as the second features. <br> 

![HDB_Pred_Two](/HDB_Pred_Two.png) <br>

<u>Conclusion: </u> <br>
Using the features detailed above, the Room Mean Square Error (RMSE) have improved to a value of $55,431.29. This indicates that the model can predict the resale value of the HDB flat with a variance of $55,431.29 from the actual price. Additionally, an R² value of 0.85 suggests that the model effectively explains 85% of the variation in the resale value of the HDB flats. <br> 
