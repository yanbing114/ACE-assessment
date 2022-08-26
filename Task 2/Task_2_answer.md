A team of plantation planners are concerned about the yield of oil palm trees, which seems to fluctuate. They have collected a set of data and needed help in analysing on how external factors influence fresh fruit bunch (FFB) yield. Some experts are of opinion that the flowering of oil palm tree determines the FFB yield, and are linked to the external factors. Perform the analysis, which requires some study on the background of oil palm tree physiology.

(refer attachment palm_ffb.csv)

![image](https://user-images.githubusercontent.com/67685003/186804769-dfad7433-6d3b-4896-ae06-fade65b208c2.png)

This dataset contain 8 numerical feature and 1 date, and has 130 samples. This dataset do not have null value.

![image](https://user-images.githubusercontent.com/67685003/186804949-fb1d6af8-d3b4-4007-b321-51b395a390c7.png)

i. The standard deviation of feature SoilMoisture, Precipitation, and	HA_Harvested is relative high.\
ii. Most of the feature has mean close with median, this means the symmetrical distribution.

Feature "Working_days" is the only discrete feature which have the unique value less than 10.\
![task_2_working_days_countplot](https://user-images.githubusercontent.com/67685003/186805831-f139fc4f-94ce-458b-94ba-5a27e1531cc8.jpg)

Here is the pairplot of the dataset.\
![task_2_pairplot](https://user-images.githubusercontent.com/67685003/186805969-00c51508-3d61-467d-a092-bb7f8b206468.jpg)

Here is the distribution histrogram of the dataset.\
![task_2_hist](https://user-images.githubusercontent.com/67685003/186806156-e2995524-91f3-4964-9dd2-2f9b3557a106.jpg)

Most features are normally distribution except "Working_days" and "FFB_Yield".

Here going to perform feature selection which with affect the FFB_Yield.

Correlation\
![Task_2_corr](https://user-images.githubusercontent.com/67685003/186806357-71b528f1-2110-4b78-b521-cb6d8ebe0a67.jpg)

![image](https://user-images.githubusercontent.com/67685003/186806474-71f75aa0-393f-4c44-a1e6-e0ebd554cefe.png)\
From here it show that, HA_Harvested, Precipitation, Working_days, Min_Temp have the high correlated with FFB_yield. This means other feature can be remove when perform machine learning, the result do not have much difference and this help to reduce the computational cost.

Embedded Methods with XGBRegressor\
![task_2_XGBR](https://user-images.githubusercontent.com/67685003/186808607-025732ea-9139-4354-bd72-31f61e4e386d.jpg)\
There slight difference between the correlation method and embedded method. However, HA_Harvested and Precipitation still have strong importance to FFB_yield as the correlation method. Average_Temp, Max_Temp, Working_days have some effect to FFB_yield.
