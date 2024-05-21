# Problem statement

Problem Statement:
In today's dynamic business environment, optimizing supply chain operations is crucial for reducing costs and enhancing customer satisfaction. To achieve this goal, it is imperative to conduct a comprehensive analysis of supply chain data to identify inefficiencies and accurately predict stock requirements.

Objective:
The primary objective of this project is to analyze supply chain data to uncover inefficiencies and predict stock needs. By doing so, the aim is to reduce operational costs and improve customer satisfaction.


# Dataset Description

OrderNumber: Unique identifier for each order.
Sales Channel: Channel through which the sale was made (e.g., In-Store, Online, etc.).
WarehouseCode: Code representing the warehouse from which the product was procured.
ProcuredDate: Date when the product was procured.
OrderDate: Date when the order was placed.
ShipDate: Date when the product was shipped.
DeliveryDate: Date when the product was delivered.
CurrencyCode: Currency used for the transaction.
_SalesTeamID: ID of the sales team involved in the transaction.
_CustomerID: ID of the customer making the purchase.
_StoreID: ID of the store where the purchase was made.
_ProductID: ID of the product being sold.
Order Quantity: Quantity of the product ordered.
Discount Applied: Any discount applied to the order.
Unit Cost: Cost of each unit of the product.
Unit Price: Selling price of each unit of the product.

# Feature engineering

Standardization: The features 'Unit Cost' and 'Unit Price' are standardized using StandardScaler(). Standardization ensures that these features have a mean of 0 and a standard deviation of 1, making them comparable and avoiding bias in the model.
Label Encoding: Categorical variables 'Sales Channel' and 'WarehouseCode' are encoded using LabelEncoder() from scikit-learn. This process assigns a unique numerical value to each category, enabling the model to process categorical data.

# Modeling

Model Used: LightGBMRegressor
Key Steps:
Data Preprocessing
Model Training
Prediction

Model Evaluation:
RMSE for Stock Prediction: 1.20 units
R2 score for Stock Prediction: 0.74
Stock Difference: 15.81 units
R2 score for Predicted Stock: 0.74

Insights:
The model explains approximately 74% of the variance in the actual stock quantities.
The average predicted stock quantity is 4.59 units, with an RMSE of 1.20 units.
The stock difference between predicted and actual quantities is 15.81 units.

Average Predicted Profit: 3417.0544117112318
R2 score: 0.9943252661949764
Profit: 12524.78936898522

