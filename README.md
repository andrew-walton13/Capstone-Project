# Capstone-Project
This was a project that I worked on as part of the Capstone Course for the MSBA I received from the University of Utah.

## Business Problem

The business problem that we were attempting to solve was to predict demand for 7 different innovation products that were proposed by a large drink manufacturer. For each of the proposed 7 innovation products, there was a list of proposed characteristics such as packaging type, manufacturer, caloric segment (diet vs regular), flavor, region, brand, etc. There was also a specific question for each product, such as when would be the best 13 week period for this innovation product, which region should we sell this to, etc. I focused on the product 4 which was called “Diet Square Mulberries.” The proposal for this product was to release it for one year in the Northern Region, so I needed to predict demand for this product if it were to be sold for one year in the Northern Region. In addition to predicting demand, I would need to make recommendations about how to best go-to-market with this product.

## Problem Solving Process

My group’s solution to this problem was a multi-step process. First, we did some initial EDA and data cleaning and engineering to make sure that we were efficiently interacting with the data. The data set was extremely large so we wanted to make sure that we have all the right data and we wanted to remove the data that we didn’t need. We also split the original data frame into a series of “innovation data sets” which were filtered data sets that were meant.  to mimic the proposed innovation products. We then took each of those innovation data sets and ran linear regression models to evaluate the effect that each predictor had on sales as well as which predictors were most statistically significant. Once we had gained some insight into the relationship between the predictors and sales, we ran XGBoost models to predict demand and make recommendations based on the demand predicted. 

## My Contributions

I was assigned to focus on the 4th innovation product specifically, which was Diet Square Mulberries. We all followed roughly the same process as described above. With my product specifically, we did see that the Mulberries flavor had shown some previous success in the Northern Region and the Northern Region was one of the most important factors to success in the model. Mulberries most successful flavor was also a sparkling water product so there was some support for going ahead with this as an innovation product. The case against moving forward with this product would be related to the Mulberries flavor generally having low unit sales, so the predictions for this product, while pretty food when compared to the other mulberries products, was very low in unit sales compared to the other innovation products.

## Business Value

Using the recommendations that our team gave will provide significant value for the sponsor company. They will be much more informed now as far as what demand to expect for the proposed innovation products and they can focus more on the products that we recommended in tier 1(products we are predicting to be most successful) vs tier 2 (products we are predicting to be less successful). We ended up putting 3 of the 7 products in tier 1 and the other 4 in tier 2. Focusing on the tier 1 products should lead to greater success for the company’s bottom line. They will be able to more properly plan what inventory is needed and do a better job of avoiding overages and shortages in inventory.

## Difficulties Encountered

We encountered quite a few difficulties with this project. First, how do we predict demand for products that do not currently exist. Second, we had very large data sets that made it difficult to load into our normal sources so we had to get creative and load the data in as more efficient file types than what was provided to us. Third, the data provided to us didn’t always give us a good way to predict demand for future products (sometimes the flavor combination was never used previously, for example). 

## Key Learnings

I learned a lot about real world problems from this project. A lot of the assignments that we do in our classes have very nice, tidy data sets that are not that big and the data is very clean and ready to be used. This was a case where we had a huge data set so we had to figure out how to work with a data set that was multiple millions of rows. We also had to figure out what to do when the dataset had a lot of data that wasn’t clear to us what it was. The item names were scrambled and randomized so we didn’t know what flavors/products they were in real life, so that added another element of the unknown to the project. It was also the first time that I think I have been asked to predict demand for non-existing products, so attempting to do that was a new challenge. Overall, I learned about how to take a real world, large scale problem and apply different methods to solve that problem.

