# Cryptocurrencies
## Overview
This project focuses on preparing an analysis of the cryptocurrencies market for potential investors. The goal of the analysis is to create a crypto investment portfolio for a fictional client “Accountability Accounting” to offer to their customers. The report generated from this project will include which cryptocurrencies are on the trading market and how they could be grouped to create a classification system for a new investment. 
The initial data will go through preprocessing to ensure it is fit for machine learning. Since the output is unknown, the models will be utilizing unsupervised learning. To group the tokes visually, a clustering algorithm will be generated. Additional visualizations and table generation will be sufficient for a dashboard presentation.
## Analysis
The data is cleaned and the “get_dummies()” function was used to create variables for text features. The data was then scaled using sklearn, and the dimensions reduced using the PCA algorithm:
![]( https://github.com/pojones/cryptocurrencies/blob/a37eae3872b6a2f47e770283116f5637c717ae44/images/deliverable1.png)
The data was then passed to a dataframe and grouped by principal components:
![]( https://github.com/pojones/cryptocurrencies/blob/a37eae3872b6a2f47e770283116f5637c717ae44/images/deliverable2.png)
An elbow curve is generated to determine the best number of clusters to apply to the cleaned dataset:
![]( https://github.com/pojones/cryptocurrencies/blob/a37eae3872b6a2f47e770283116f5637c717ae44/images/deliverable3.png)

## Results
After sklearn groups the tokens into four classes, we visualize the output:
![]( https://github.com/pojones/cryptocurrencies/blob/a37eae3872b6a2f47e770283116f5637c717ae44/images/deliverable4Scatter3d.png)
Classes zero, two, and three have similar values for total coins supplied. However, class one is most notable; it has both a high number of coins supplied and a high number of coins mined. 
![]( https://github.com/pojones/cryptocurrencies/blob/a37eae3872b6a2f47e770283116f5637c717ae44/images/deliverable4scatterTotals.png)
