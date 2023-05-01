### **Sales Forecasting**
In this project, we use statistical and machine learning forecasting methods to attempt to accurately forecast the next 21 days of sales for every product listed in our dataset. This project is drawn from a kaggle competition, the link to which can be found here:
https://www.kaggle.com/competitions/ysc4224-2023-final-project/overview


Our method explores two stastical models, ARIMA and ETS, and a machine learning model, XGBoost. ETS provided the best results, followed up by XGBoost, then ARIMA. The notebook containing the code and analysis of the different models used for each method can be found in their respective folders. It should be noted that the data required to build the code is included in the data folder and other files that are loaded in the code are results from large dataframes being downloaded as csv files to reduce overhead. Additionally, the summary of our findings and the visualization of our different models can be found in the presentation pdf.



#### Next Steps
Future directions with this project would be acquiring the computational capacity to run our model with the clusters obtained from DTW (for XGBoost and ARIMA) as the distance from each item to its dtw cluster is regularised for time-series data. An ideal scenario would be to run our statistical models for each item without time-series clustering.

For the current models, we observed that XGBoost did not perform the best as we expected it to. This may be because there is a lack time-independent features that can provide more information for tree-based learning. Such features include inventory, reviews or sentiment - these may offer insights such as the underlying affects of features on sales. Additionally, if we are allowed the computational capacity, we could incorporate ensemble learning using different machine learning models in our method.