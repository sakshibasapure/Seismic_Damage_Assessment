# **2015 Gorkha Earthquake: Seismic Damage Assessment**

### **Richter's Predictor: Modeling Earthquake Damage**


---




The main aim is to predict the level of damage to buildings caused by the 2015 Gorkha earthquake in Nepal based on aspects of building location and construction. The dataset used is ***Richter's Predictor: Modeling Earthquake Damage*** which is present in [datadriven.org](https://www.drivendata.org/competitions/57/nepal-earthquake/) competition. This data was collected by Kathmandu Living Labs and the Central Bureau of Statistics, and contains valuable information on earthquake impacts, household conditions, and socio-economic-demographic statistics.






Problem statement is to predict the ordinal variable **damage_grade**, which represents a level of damage to the building that was hit by the earthquake. There are 3 grades of the damage:
1. represents low damage
2. represents a medium amount of damage
3. represents almost complete destruction




### **Steps**
1. Import Libraries and Dataset
2. Exploratory Data Analysis
> * Check null and missing values
> * Check unique values
> * Visualization between features and class label
3. Data Preproccesing
> * Label Encoding 
> * Outlier Removal using IQR
4. Model Evaluation
> * Random Forest without sampling
> * Random Forest with SMOTE sampling
> * Random Forest with TomekLins sampling
> * Random Forest with SMOTETomek sampling
> * Random Forest with SMOTE-ENN sampling

To measure the performance of our algorithms, F1 score is used as it balances the precision and recall of a classifier. Traditionally, the F1 score is used to evaluate performance on a binary classifier, but since we have three possible labels we will use a variant called the micro averaged F1 score

Of all the results obtained, we achieve the best performance with **Random Forest classifier using SMOTE-ENN sampling method** with best score of **77.58%**. 




