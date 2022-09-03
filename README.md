# Instacart Market Basket Analysis

Data can be downloaded here: Kaggle : https://www.kaggle.com/c/instacart-market-basket-analysis/data

## 1.  Project Overview

Within two past year’s covid-19 pandemic, there’s a rapid growth on online shopping no longer concentrated on Amazon.com, but also other new grocery online shopping websites like Instacart. Instacart provides a new shopping experience for customers to buy grocery items online from different department stores such as Costco, Safeway, Walmart, Target and so on. It shows the convenience of the same-day grocery delivery and pick-up service especially during COVID-19. There’s no need to go to grocery stores for customers to shop their favorites and save their time. It creates an easier way to fill peoples’ refrigerator and stomach with their personal flavors. With the business growth, the company will need more attention on customer’s behavior to dig more valuable information on business development. Our project will bring great business value and will unlock the hidden business insights from Instacart customers’ purchase history and the result of this project could be used to improve Instacart’s profitability and increase customer satisfaction.

## 2. Problem Statement

The goal of the project is to use the anonymized data on customer orders over time to predict which previously purchased products will be in a user’s next order. In this project we will discover clusters and subgroups of customers with similar purchase behavior using segmentation, association rules and prediction models and visualize the data to create relevant recommendations focused at improving revenue and customer experience. If we can know the customer who purchased one product and he/she is more likely to purchase another product, we can suggest the company to target those products to the grouped customers. Therefore, finding out what products that Instacart customers frequently purchase together, it will become possible to give future marketing recommendations to boost sales growth and make business decisions.

## 3. Data Exploration

Before explore data, we do preprocessing the dataset. We use Matplotlib and Seaborn for our visualization. 
Some meaningful insights that we have: Best selling products, the frequent words describe the products, the most ordering in Aisle, number of item in each department, the most ordering in the department, reorder ratio per department/aisle, relationship between reorder and add-to-cart.

## 4. K-Mean Clustering Analysis

By applying K-means clustering, we map the users in five groups, who are new users, who purchase daily fresh products and dairy, who are majorly families that have babies, who like to eat on the go and easy cooking items, and who rely more on frozen food. We can target different cluster customers to promote different aisles products to make them purchase more food.

## 5. Association Rule Mining

We applied Apriori association rules to find the most frequent item bundles. We are able to fetch various product recommendations based on a selected product.

## 6. Models

Before building the model, we create 11 predictor variables, next we split train set and test set.
Since the dataset is imbalance and complicated, we use XGboost and LightGBM models for our project.
The perfomance metrics that we use: confusion matrix, precision, recall and F1-score.

## 7. Prediction

XGBoost model has the higher F1-Score, we use it to predict on the future orders.
Prediction is saved as a csv file named: reorder_prediction.csv

Team members: Duyen Thanh, Neha Palnati, Vanshika Gupta, Xiangnan Cui
