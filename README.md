# King County Housing Analysis with Multiple Linear Regression.

Author: Clyde Ochiieng

## Overview

In the grand scheme of things, a youthful duo is in the midst of orchestrating the sale of their abode, harboring aspirations to elevate its market worth with minimal financial resources allocated for refurbishments. In a strategic move, the couple has opted to employ Multiple Linear Regression Modeling to meticulously scrutinize and prognosticate house sales trends in King County, leveraging specific attributes or variables. This analytical approach is poised to empower them with insights to navigate the market intelligently, thereby facilitating judicious decisions for maximizing profitability.

Following a rigorous evaluation process and numerous iterations of our linear regression models, it has been ascertained that the dimensions of living space and the quality grade of the construction exhibit the most pronounced correlation with an augmented selling price of the property.
## Business Problem


The business quandary at hand revolves around providing insightful counsel to prospective homeowners regarding the potential impact of home renovations on the estimated value of their properties, alongside quantifying the magnitude of such enhancements.

In addressing this issue, we aim to equip homeowners, both buyers and sellers, with invaluable insights that can inform their decisions in the real estate market. Our focus lies in scrutinizing key factors such as building grade and square footage of living space, among others, to unveil the correlations that exist between these features and home sale prices. This comprehensive analysis seeks to elucidate the most influential attributes driving property values, thereby empowering stakeholders to make informed and strategic decisions pertaining to their real estate endeavors.
### Hypothesis

In crafting our hypotheses, we put forward the following propositions:

Null Hypothesis (H0): Within our model, we posit that there is an absence of any substantial association between the independent variables and the dependent variable (target).

Alternative Hypothesis (H1): Contrarily, we assert that a meaningful relationship does exist between the independent variables and the dependent variable (target) within our model.

To guide our analytical journey and ensure robust conclusions, we have established a significance level (alpha) of 0.05. This chosen threshold will serve as a pivotal benchmark against which we evaluate the statistical significance of our findings and shape our ultimate recommendations for stakeholders.

### Questions to be analyzed

et's articulate the questions we aim to explore through our analysis:

Q1: Which features show the strongest correlation with the price of a home?

Q2: Among the predicting variables, which features exhibit the most significant correlations with each other?

Q3: What combinations of features offer the most reliable predictions for home prices?

These questions form the cornerstone of our investigation, guiding our efforts to uncover key insights that will assist homeowners, buyers, and sellers alike in navigating the complex landscape of real estate with confidence and clarity.

## Data Understanding

In our quest to gain a comprehensive understanding of the data under scrutiny, we turn our attention to the King County Housing dataset. This dataset encapsulates a wealth of information pertaining to over 21,000 homes situated in King County.

Each entry in the dataset provides detailed insights into various attributes of the homes, encompassing factors such as the number of bedrooms, bathrooms, and floors, as well as the square footage of both living space and lot, the zip code, building grade, and condition, among others.

The dataset comprises a multitude of features, each potentially contributing to the final sale price of homes in King County. Below, we delineate the descriptions of these features, laying the groundwork for a thorough exploration and analysis.

## Methods


The dataset underwent thorough exploration and investigation using core principles of Exploratory Data Analysis (EDA). Object data types were converted to integers using techniques like the split function or mapping. Subsequently, redundant data, including duplicates and irrelevant columns, was removed. Outliers were handled by excluding data points exceeding 3 standard deviations from the mean, tailored to the specific criteria under review.

Descriptive statistics and visualizations played a crucial role in uncovering trends and identifying key factors essential for the development of profitable homes. Multiple linear regression models were constructed to identify the strongest correlations within the dataset. An iterative approach was adopted for model-building, with each model being evaluated meticulously. The process involved revisiting the data repeatedly to identify opportunities for enhancements or modifications aimed at achieving a more effective model.

## Results


### Visual 1
![fig1](./images/grade vs price.png)

A discernible positive correlation exists between building grade and home sale price. As the grade designation escalates on the scale of 1 to 13, the corresponding house price demonstrates a concurrent increase.


![fig2](./images/sqft_living vs price.png)

T# Exploring the Positive Relationship between Square-Footage of Living Space and Home Sale Price

Our analysis unveils a strong positive correlation between the square footage of living space and the sale price of homes. As the living space expands, so does the corresponding price of the house.

## Key Questions Investigated

### Question 1: Features with the Strongest Impact on Home Price
We identified that the grade of the house, square footage of living space (sqft_living), and the number of bathrooms have the most significant correlation with home price.

### Question 2: Features Exhibiting Strong Correlations with Other Predictive Variables
We found no features with correlations exceeding 0.75, indicating no significant multicollinearity issues. However, sqft_living and grade demonstrate the highest correlation within our dataset.

### Question 3: Best Feature Combinations for Accurate Price Predictions
Our analysis suggests that a multiple regression model incorporating grade, sqft_living, and bathrooms offers the best fit for predicting house prices. These features not only show high correlation with price but also exhibit low multicollinearity, collectively explaining over half of the price variability.

## Summary of Modeling Efforts

We developed six models to predict housing prices, each yielding valuable insights:

- Model #1: Basic model using the two most correlated features resulted in an R2 of 0.486.
- Model #2: Improved model with train-test split and one-hot encoding applied to the condition feature achieved an R2 of 0.605.
- Model #3: Model dropped multicollinear feature sqft_living, resulting in an R2 of 0.467.
- Model #4: Utilized significant features sqft_living, grade, and bathrooms, resulting in an R2 of 0.485.
- Model #5: Employed relevant features with one-hot encoding on the condition feature, resulting in an R2 of 0.609.
- Model #6 (Final Model): Incorporated all techniques, yielding the highest R2 of 0.871.

## Evaluation and Conclusion

The final model's predictability significantly increased to 0.871, indicating its effectiveness in predicting housing prices. Recommendations derived from our analysis include increasing square footage, aiming for higher building grades, and adding bathrooms to the property, all of which contribute to higher sale prices.

For further inquiries, please contact:

Clyde Ochieng at <dosclyde@gmail.com>

## Repository Structure

- README.md: Top-level README for reviewers
- King_County_Housing...ipynb: Jupyter notebook
- house_slides.pdf: Project presentation slides (PDF)
- house_notebook.pdf: Jupyter notebook (PDF)
- data: Data directory (sourced externally or generated from code)
- images: Image directory (sourced externally or generated from code)
