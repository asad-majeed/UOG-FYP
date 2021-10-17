
## 1. Data Collection:

The first step after understand a business problem, we need to collect raw data. It is either from company databases,3rd party api,cloud or by using web scrapping. for this project I have collected a data from kaggle. the link is given below. After getting a dataset, we need to understand a complete dataset.
https://www.kaggle.com/spideysloth/pakwheels-cars-dataset

## 2. Statistical And Graphical analysis:

In this step we will do some statiscal and graphical analysis to understand the distribution of the data, to understand a relationship between independent and dependent variables to decide our model. if the data has linear relationship between independent and dependent variables then we can use linear regression. but in this project you will see a data is not follow a linear relationship so we have to choose non linear model that perform well in this scenario. we have derived 2 new attributes from the Name Column.
             
## 3. Feature Engineering:

Since we have huge amount of dataset almost more than 56000 records from train and test dataset, we have very less number of missing values in the dataset I will remove it.in case of categorical features encoding. since we a lot of catogories in model, brand,model or city etc, so in order to avoid curse of diemensionality problem we will do label encoding. but in order to get better accuracy from model we have to try all different different techniques including for imputation,encoding,transformation. incase of transformation I have convert some features like price from object type to int type and did some data cleaning in this column which have records like "Call for price".Because our model will only accept numbers and help us to do a prediction.I have also removed some duplicates values from the dataset.

## 4. Feature Selection:

I have used all the features before building my model according to the requirements.but sometimes we have to build a model after finding out some important features that help us to do prediction. we no need to dump all the features in the model for training.

## 5.Train And Test Split.

I have train my model on 80% and 20% keep for test. But Try Not to use this test dataset for testing that cause a biased result because it is coming from same population,so try to use another dataset from other population for user accepting testing. and by the way this dataset will be given by stakeholder/business owner for true validation of the model.

## 6. Model Building:

In this project you will see that I have used different different models for training. because some models gives me a bad accuracy. So I have choose a one which will gives me a better accuaracy. so in this case i have used Ensemble Technique(Random Forest Regression) for my final model building after true validation. and this is the only model that we have get as our final model after reading 2 research paper from the internet related to this problem.
 
 ## 7. Model Testing:

It is very very important step. Because without user accepting testing,  we will not deploy it into the production. for testing data I will apply all data preprocessing step that we had actually applied during training my model. 
                            
