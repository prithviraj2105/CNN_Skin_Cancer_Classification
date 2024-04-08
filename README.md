# CNN Assignment
> CNN model to classify types of skin cancer based on skin images.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- This project is part of course study assignment. The course is Advanced Certification Program in Machine Learning and Deep Learning (ACP in ML & DL) conducted by IIIT Banglore. The project is building a Ridge and Lasso Regression model for predicting House Price.
- A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. The management aspires to understand how exactly the prices vary with the housing features. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns.

The company wants to know:
- Which variables are significant in predicting the price of a house, and
- How well those variables describe the price of a house.

The company has collected a data set from the sale of houses in Australia.

The requirement is to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions

We have chosen Lasso Regression model with optimal alpha=0.001 as final model because as per analysis this is the most robust and generalisable model.
This model has far less number of features which translates to reduction in complexity. The model is simpler and thus interpretable.
The difference between R^2 of Train and Test data is comparatively less in this model. The metrics data shows that though the model's accuracy is slightly low on training data it is more generalisable and performs better on unseen data.
#### Train data

r2 score = 0.8748348448916363 rss = 3.989855681947641 mse = 0.004447999645426579 rmse = 0.06669332534389463

#### Test data
r2 score = 0.7658494795148396 rss = 3.239954389683936 mse = 0.008415465947231002 rmse = 0.09173584875734787

Based on the final model we can say that the model describes 87% of the variability in price of house and also has decent predictive power with 0.77 r2 score on test data.

The top 5 features which are most significant in determining the House price are;
- ‘OverallQual’ (Rating of the overall material and finish of the house) has positive correlation with Sale Price.
- ‘GrLivArean’ (living area above grade (ground) in square feet) has positive correlation with Sale Price.
- ‘TotalBsmtSF’ (Basement area in square feet) has positive correlation with Sale Price.
- ‘GarageArea’ (Size of garage in square feet) has positive correlation with Sale Price.
- ‘TotRmsAbvGrd’ (Total rooms above grade (does not include bathrooms)) has positive correlation with Sale Price.

The analysis has shown that the most obvious factors have contributed to the sale price of the house. We can see that the quality of the material and finish of the house has highest impact on the sale price, price increases as the rating of the quality increases. The other significant factors affecting the price are the size of living area above ground, basement area, garage area and number of rooms above ground.

The housing company should consider concentrating on houses with high quality material and finish.
<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Jupyter Notebook - version 6.5.4
- Python - version 3.11.5
- numpy - version 1.24.3
- pandas - version 2.0.3
- seaborn - version 0.12.2
- matplotlib - version 3.7.2

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project is done with reference to a example 'Predict the sales given the spend on marketing' covered in the Advanced Regression module.


## Contact
Created by [@prithviraj2105] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project --># CNN_Skin_Cancer_Classification
