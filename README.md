# price-prediction-capstone-python
This was my final Capstone project for the MIT course Applied Data Science Program: Leveraging AI for Effective Decision-Making. The objective was to come up with a pricing model that can eﬀectively predict the price of used cars and can help a business in devising profitable strategies using diﬀerential pricing.

## **Problem Definition**

### **The Context:**

 - **Why is this problem important to solve?**
 
The used car market in India has outgrown the new car market in recent years, with over 4 million second-hand cars sold in 2018-19 compared to 3.6 million new cars. As consumer preference shifts toward more affordable pre-owned vehicles, accurate and transparent pricing becomes critical.
Unlike new cars, where pricing is standardized by manufacturers, used car prices are influenced by numerous variables (e.g., mileage, brand, model year), creating high uncertainty for both buyers and sellers. This unpredictability can lead to mistrust, underpricing or overpricing, and inefficient market behavior. A data-driven approach to pricing can help bring consistency and reliability to this growing industry.

### **The objective:**

 - **What is the intended goal?**
 
 The primary goal is to develop a predictive pricing model that estimates the fair market value of used cars based on various features. This model will help sellers price vehicles more accurately, allow buyers to make more informed decisions, and enable the company (Cars4U) to implement profitable, data-backed pricing strategies.

### **The problem formulation**:

- **What is it that we are trying to solve using data science?**

We are formulating this as a supervised regression problem, where the task is to predict the selling price of a used car based on features such as year, brand, fuel type, transmission, mileage, and other specifications. This will be done using historical data to train machine learning models that can generalize well to unseen data. To tackle this, we implement and compare multiple machine learning models, including:
- **Linear Regression** – for a simple, interpretable baseline  
- **Ridge & Lasso Regression** – to handle multicollinearity and feature selection  
- **Decision Tree** – to capture non-linear patterns in the data  
- **Random Forest** – a model that improves performance and reduces overfitting

By training and evaluating these models, we aim to:
- Identify which approach best balances accuracy and interpretability
- Understand how different features impact car pricing
- Build a solution that can be deployed or scaled to assist sellers and the business with dynamic pricing strategies


### **Data Dictionary**

**S.No.** : Serial Number

**Name** : Name of the car which includes Brand name and Model name

**Location** : The location in which the car is being sold or is available for purchase (Cities)

**Year** : Manufacturing year of the car

**Kilometers_driven** : The total kilometers driven in the car by the previous owner(s) in KM

**Fuel_Type** : The type of fuel used by the car (Petrol, Diesel, Electric, CNG, LPG)

**Transmission** : The type of transmission used by the car (Automatic / Manual)

**Owner** : Type of ownership

**Mileage** : The standard mileage offered by the car company in kmpl or km/kg

**Engine** : The displacement volume of the engine in CC

**Power** : The maximum power of the engine in bhp

**Seats** : The number of seats in the car

**New_Price** : The price of a new car of the same model in INR 100,000

**Price** : The price of the used car in INR 100,000 (**Target Variable**)
