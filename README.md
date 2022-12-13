# Big-Data-Group-8
This project is a part of the ITCS 6100 - Big Data Analytics for Competitive Advantage course from the University of North Carolina at Charlotte.
# Deliverable 1

## Team Members
* Kousik Varma Dandu
* Dinesh Reddy Chinnamallaiahgari
* Reddy Sai Krishna Sanda
* Sheshi Rekha Guntuka

## Communication plan
Zoom meetings, Atkins Library, Slack. 
We plan to communicate 3 times per week through zoom or in-person meetings based on the availability of the group members. The meetings will last for 2-3 hrs each. 

## Dataset
Canvas-sample-housing.csv: In this dataset, we will find data about the characteristics associated with a particular housing price. We can use this dataset to predict housing prices. With this dataset, use the Numeric prediction model type. The link to the dataset can be found here. https://www.kaggle.com/datasets/camnugent/california-housing-prices

## Selection of Data
California Housing Prices Data

https://www.kaggle.com/datasets/camnugent/california-housing-prices

Description:  ```California housing prices Dataset```

Resource type: 
```S3 Bucket```

Amazon Resource Name (ARN): 
```arn:aws:s3:::housee```

AWS Region: 
```US East (N. Virginia) us-east-1```

## Business Problem or Opportunity, Domain Knowledge 
As the population increases day-by-day the demand for houses increases side by side. Predicting housing prices based on the characteristics of a locality is the task at hand. During the COVID-19 pandemic era, the demand for houses has increased rapidly. During this process, we should identify the most significant features in the California Housing Dataset. The real Estate domain is the most earning field in the world. Most realtors may not be able to provide a good house to the customers. We will be using machine learning techniques to predict California housing prices.

## Research Objectives and Questions
What is the actual value of the price and predicted value of the price of the house?

Find the location where the highest total rooms are located?  

What is the median house value in accordance with median housing age in different ocean proximities? 

How median house value can be compared with median house income?

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Deliverable 2

## Data Understanding

a) Exploratory Data Analysis

Exploratory Data Analysis was done through AWS Sagemaker. View the rendered file here: Exploratory Data Analysis(link need to attach)

b) Dashboard

Dashboard instances were created using AWS Quicksight and rendered as PDF files. The PDF extracts are available below. Additionally, these dashboards are analyzed in the Results section as a tool for evaluating the research objectives and questions.

[Click Here For Dashboards](https://github.com/saikrishnasanda/bigdata/blob/main/Project%20Files/AWS%20Quicksight/AWS%20Quicksight.pdf)



## Data Preparation
At every stage of the project, data preparation was done, including an initial study of the dataset structures listed in the Open Dataset Registry. Data preparation tasks include reading column data correctly based on the tool being used, taking into account anomalous data, erroneous values, manipulating the data, and more.  We found some null values in total_bed_rooms column in the dataset and filled that with the median of the values from the same column.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Deliverable 3  

## Analytics, Machine Learning
Using Amazon SageMaker, we performed Machine learning and analytics for predicting the results. We used different types of barcharts, scatter plots, Heatmaps to view the results. The dataset was train and tested with random forest and CatBoost algorithms and printed the root mean square(RMSE) and R-square. These two gave the best results. So, we combined the two models to get final prediction. 

[Click Here to View the results](https://github.com/saikrishnasanda/bigdata/blob/main/Project%20Files/AWS%20Sagemaker/house%20price%20prediction.ipynb)

## Evaluation and Optimization
Performing machine learning on AWS will boosts the running computations. The machine learning model like Random forest which helps to find the predicted median house value in the data, along with random forest we used Catboost which adds best solutions with out parameter tuning that reduces time spent on parameter tuning because CatBoost provides effective results with default parameters. Using Scatter plot for visualizing the predicted house values, based on the positive correlations of the plot helps the data scientist to analyse the stats for better understanding. By optimizing the models for the best fit, a scatter chat can help in setting up models

## Results
### What is the actual value of the price and predicted value of the price of the house?
Here the main aim to display the results by showing the comparision between the actual median_house_price vs predicted median_house_price. The scatter plot explains all the comparison between the values. The results are displayed below.
![alt text](https://github.com/saikrishnasanda/bigdata/blob/main/Project%20Files/Results/prediction.png)


### Find the location where the highest total rooms are located?
Using this visualization box we can understand at what area of location have the highest number of total rooms. We can see from below bar chart that <1H Ocean from ocean proximity column (location of houses located with respect to ocean) area has the highest number of total rooms. 

There are a total number of 9,034 bedrooms in total in that area. So we can make assumption that this area contains the big houses or many houses.
![alt text](https://github.com/saikrishnasanda/bigdata/blob/main/Project%20Files/Results/Highest%20rooms%20located.jpg)

### What is the median house value in accordance with median housing age in different ocean proximities?


