# Customer-Personality-Analysis-

Customer Personality Analysis is a detailed analysis of a company’s ideal customers. It helps a business to better understand its customers and makes it easier for them to modify products according to the specific needs, behaviors and concerns of different types of customers.
Customer personality analysis helps a business to modify its product based on its target customers from different types of customer segments. For example, instead of spending money to market a new product to every customer in the company’s database, a company can analyze which customer segment is most likely to buy the product and then market the product only on that particular segment.

#  Content
**Attributes**

**People:**
- **ID**: Customer's unique identifier
- **Year_Birth**: Customer's birth year
- **Education**: Customer's education level
- **Marital_Status**: Customer's marital status
- **Income**: Customer's yearly household income
- **Kidhome**: Number of children in the customer's household
- **Teenhome**: Number of teenagers in the customer's household
- **Dt_Customer**: Date of the customer's enrollment with the company
- **Recency**: Number of days since the customer's last purchase
- **Complain**: 1 if the customer complained in the last 2 years, 0 otherwise
  
**Products:**
- **MntWines**: Amount spent on wine in the last two years
- **MntFruits**: Amount spent on fruits in the last two years
- **MntMeatProducts**: Amount spent on meat in the last two years
- **MntFishProducts**: Amount spent on fish in the last two years
- **MntSweetProducts**: Amount spent on sweets in the last two years
- **MntGoldProds**: Amount spent on gold in the last two years

**Promotion:**
- **NumDealsPurchases**: Number of purchases made with a discount
- **AcceptedCmp1**: 1 if the customer accepted the offer in the 1st campaign, 0 otherwise
- **AcceptedCmp2**: 1 if the customer accepted the offer in the 2nd campaign, 0 otherwise
- **AcceptedCmp3**: 1 if the customer accepted the offer in the 3rd campaign, 0 otherwise
- **AcceptedCmp4**: 1 if the customer accepted the offer in the 4th campaign, 0 otherwise
- **AcceptedCmp5**: 1 if the customer accepted the offer in the 5th campaign, 0 otherwise
- **Response**: 1 if the customer accepted the offer in the last campaign, 0 otherwise

**Place:**
- **NumWebPurchases**: Number of purchases made through the company’s website
- **NumCatalogPurchases**: Number of purchases made using a catalog
- **NumStorePurchases**: Number of purchases made directly in stores
- **NumWebVisitsMonth**: Number of visits to the company’s website in the last month

- **NumWebVisitsMonth**: Number of visits to the company’s website in the last month

## Task ##
Figuring out who are the wealthy customers is any company's dream. The "whales" have more to spend and are arguably less discounted. I will use Radom Forest to predict which customer.

- **Prepare Data Set**
  Remove variables that don't make sense to be there, and transform some that need transformation.
(e.g., Birth Year). Additionally, make sure you only have numeric variables and remove NAs. Finally, create a Training and Test set.

- **Random Forest Model**
  Remove variables that don't make sense to be there, and transform some that need transformation.
(e.g., Birth Year). Additionally, make sure you only have numeric variables and remove NAs. Finally, create a Training and Test set.

- **Accuracy Assessment**
  How good is your model? Predicting income is an important task, and thus, being good at it is pivotal.

- **Model Tuning**
    Build a process to tune the optimal number of trees. This is an introduction to parameter tuning. The goal is to have the skill to understand advanced analytical projects.
  
- **Generate Insights**

![image](https://github.com/MuyiwaNau/Customer-Personality-Analysis-/assets/34709932/8b217645-48a4-4d6e-8f8e-cd2c05d722a3)


**Random Forest Model:**

Random Forest is an ensemble learning technique used in machine learning for classification and regression tasks. It is constructed from multiple decision trees to improve the model's accuracy and reduce overfitting.

**Key Features:**
- Ensemble Learning: Random Forest combines the predictions of multiple decision trees to make more accurate predictions.
- Decision Trees: Each tree is constructed using a random subset of the data and features, improving diversity.
- Bagging: Random Forest employs bagging (Bootstrap Aggregating) to create diverse datasets for each tree.
- Feature Importance: It measures feature importance, allowing you to identify the most influential variables in your dataset.

Advantages:
- Robust to Overfitting: Random Forest is less prone to overfitting than individual decision trees.
- High Accuracy: It often delivers high predictive accuracy due to its ensemble nature.
- Handles Both Classification and Regression: It is versatile and can be used for various machine-learning tasks.

	Usage Example:
	```python
	#Model
	from sklearn.ensemble import RandomForestRegressor
	model = RandomForestRegressor(n_estimators = 300,
	                              random_state =1502)
	model.fit(X_train, y_train)

**Resources** 
- **Marketing_campaign.csv**
- **Python**
