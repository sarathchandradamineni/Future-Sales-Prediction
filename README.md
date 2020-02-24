# Future-Sales-Prediction
The aim of the project is to develop a machine learning model that can predict the sales of the product from different outlets. Data contains 12 attributes and 8523 instances
Step 1: Dealing with null values In the data, the attributes 'Item_Weight' and 'Outlet_Size' have null values. These null values have to be replaced with the most promising values. Attributes ‘Item_Weight’, ‘Outlet_Size’ have 17%, 28% of null values respectively
Step 2: Variance, Correlation Checking Attribute with very small variance won't serve well, so removing those attributes makes the training process simple. Two attributes with high correlation will work similarly. So, removing one attribute will better serve our purpose. 
Unfortunately, none of these properties are present in the data. 
Step 3: Handling Redundant Values Attribute 'Item_Fat_Content' has redundant values such as 'LF,' 'low fat'  for 'Low Fat', and 'reg' for 'regular.' 
So, these values have to be replaced properly. 
Step 4: Feature Engineering The minimum value of the attribute 'Item_Visibility' is zero. This makes no sense. So replacing zeros with average values group by 'Item_Identifier' will give better results. 
Determining the number of years of operation from 'Outlet_Establishment_Year' and creating new column 'Years_Of_Operation' will give better results 
Step 5: Scaling the data In order to make the training process simple and fast, scaling of data is needed.   

Training and Testing K-fold cross-validation technique used to divide the training and testing the data. In which data will be divided into a predefined number of folds so that one fold is used for testing and remaining folds are used for training purposes, This process is done for k times. 
K-fold cross-validation technique allows all the observations for training and testing. 
Moreover, the K-fold validation technique prevents the risk of overfitting during continuous testing.

Results:The accuracy obtained and time taken by the two algorithms for the ten folds with K-fold cross validation technique are the results of the project. 

Conclusion:Random Forest is more accurate when compared to the linear regression algorithm, but on the other hand, the random forest takes more time for training the model, but linear regression takes very little time to train the model. 
