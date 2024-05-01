# Phase 2 Project Description
Kings County Housing Analysis with Multiple Linear Regression
Overview
A real estate agency in Kingsway seeks to determine the contributing factors that affect the price of houses to make improvements where necessary. They want to employ an analytical approach rather than sentimentality before arriving at a decision. Multiple linear regression has been used for this project to understand how various features affect their pricing to better their services.

Business Problem
In the face of market fluctuations and heightened competition within the real estate sector, our agency is grappling with pricing volatility, which poses significant challenges for our agents in devising effective business strategies. We seek strategic guidance to optimize our purchasing and selling endeavors, prioritizing informed decision-making to identify key areas of focus that promise maximum returns on investment.

Objectives
To determine the key factors influencing house prices.
To develop multiple linear regression models to predict house prices based on relevant features.
To use insights from the regression analysis to optimize pricing strategies for both purchasing and selling properties.
Hypothesis
Null Hypothesis: There is no relationship between our independent variables and our dependent variable.
Alternative Hypothesis: There is a relationship between our independent variables and our dependent variable.
Data Understanding
In this project, we utilized the King County House Sales dataset, which serves as the foundational dataset for our analysis. It was sourced from Kaggle. The dataset encompasses comprehensive information regarding house sales within King County, Washington, USA. It comprises a diverse array of features, including the number of bedrooms, bathrooms, square footage, as well as geographical and pricing details of the properties sold. This dataset is frequently employed in data science and machine learning endeavors, particularly for predictive modeling tasks such as regression analysis aimed at forecasting house prices based on the provided features.

King County Housing Data Columns
The column names contained in column_names.md are:

id: A unique identifier for each house sale.
date: The date when the house was sold.
price: The sale price of the house, serving as the target variable for predictive modeling.
bedrooms, bathrooms, sqft_living, sqft_lot: Numerical features representing the number of bedrooms and bathrooms, as well as the living area and lot area of the house, respectively.
floors: The number of floors in the house.
waterfront, view, condition, grade: Categorical features describing aspects such as waterfront availability, property view, condition, and overall grade assigned to the housing unit.
yr_built, yr_renovated: Year of construction and renovation of the house.
zipcode, lat, long: Geographical features including ZIP code, latitude, and longitude coordinates.
sqft_above, sqft_basement, sqft_living15, sqft_lot15: Additional numerical features providing details about the house's above-ground and basement square footage, as well as living area and lot area of the nearest 15 neighboring houses.
Data Loading and Preparation
We load the dataset and prepare it for analysis by performing data cleaning tasks such as handling missing values and outliers.

Exploratory Data Analysis (EDA)
We conduct exploratory data analysis to gain insights into the dataset's characteristics and relationships between variables. This involves visualizations such as histograms, box plots, and correlation matrices.

Data Analysis
We calculate statistics for numeric columns and explore relationships between categorical features and the target variable (house prices).