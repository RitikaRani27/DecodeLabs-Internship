# Project_1_Advanced_EDA_&_Feature_Engineering

## Project Overview

This project was completed as part of the **DecodeLabs Data Science Internship**. The objective of this project was to transform a raw e-commerce transaction dataset into a clean, structured, and machine-learning-ready dataset by performing data preprocessing, exploratory data analysis (EDA), outlier detection, and feature engineering.

The dataset contains customer order details, including product information, purchase quantity, pricing, payment methods, order status, shipping details, and customer acquisition sources.

## Dataset Features

The dataset includes the following attributes:

* **OrderID** – Unique identifier for each order
* **Date** – Date of order placement
* **CustomerID** – Unique identifier for customers
* **Product** – Product purchased
* **Quantity** – Number of items purchased
* **UnitPrice** – Price of each item
* **ShippingAddress** – Customer delivery location
* **PaymentMethod** – Method used for payment
* **OrderStatus** – Current status of the order
* **TrackingNumber** – Shipment tracking information
* **ItemsInCart** – Number of items added to the cart
* **CouponCode** – Discount coupon applied during purchase
* **ReferralSource** – Source through which the customer reached the platform
* **TotalPrice** – Total value of the order

## Project Objectives

* Analyze the structure and quality of raw e-commerce data.
* Identify and handle missing values and inconsistencies.
* Detect and remove outliers from numerical features.
* Create new meaningful features to improve data analysis.
* Prepare the dataset for future machine learning and predictive modeling tasks.

## Project Workflow

### 1. Exploratory Data Analysis (EDA)

* Examined dataset structure, feature types, and statistical summaries.
* Analyzed customer purchase behavior and order patterns.
* Visualized relationships between variables such as quantity, pricing, and order value.
* Identified data quality issues including missing values and unusual observations.

### 2. Data Cleaning and Preprocessing

* Handled missing values using suitable statistical imputation methods.
* Checked and removed duplicate records.
* Corrected inconsistencies in data formatting.
* Converted date information into useful components for analysis.

### 3. Outlier Detection and Removal

* Identified extreme values in numerical columns such as:

  * Quantity
  * UnitPrice
  * TotalPrice
  * ItemsInCart
* Applied the **Interquartile Range (IQR)** method to detect and remove outliers.
* Improved dataset reliability and consistency.

### 4. Feature Engineering

Created new predictive features from existing data:

* **PricePerItem** – Calculated the average price per item purchased.
* **ExtraCartItems** – Identified additional items beyond the main purchase quantity.
* **OrderMonth** – Extracted the month from the order date.
* **OrderDay** – Extracted the day of the order.

These features provide additional insights into customer purchasing behavior and can support future machine learning models.

## Data Visualization

Performed visual analysis using graphs and charts to understand:

* Product sales patterns
* Customer purchasing trends
* Price and quantity distributions
* Relationships between order features

## Technologies Used

* Python
* Google Colab
* Pandas
* NumPy
* Matplotlib
* Seaborn

## Files Included

* `Project_1_Advanced_EDA_&_Feature_Engineering.ipynb` – Complete Google Colab notebook
* `Dataset for Data Analytics.csv` – Raw e-commerce dataset
* `Cleaned_Dataset.csv` – Processed dataset ready for machine learning

## Outcome

The project successfully converted a raw e-commerce dataset into a clean and structured dataset by applying data cleaning, exploratory analysis, outlier handling, and feature engineering techniques. The final dataset is optimized for further analysis and can be used as a foundation for customer behavior analysis, sales prediction, and machine learning applications.
