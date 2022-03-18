#Bertelsmann/Arvato Customer Segmentation Capstone Project
This is a project done as capstone final project for a data science nano-degree program with Udacity. 

#What is the Bertelsman-Arvato company? 
They are German company that provides services in customer support, information technology, logistics, and finance. 

#What is the goal of the project? 
The goal is to identify potential customers for a mail order catalog of organic and healthy products. It would not be cost efficient to send out 
catalogs to every household throughout Germany, so a more profitable approach is to target which households have would be most likely to shop from a 
catalog, saving a lot of time, money, and resources in the advertising process.

#What data is provided
Four data sets are provided, ‘azdias.csv’ provides demographics data for the general population of Germany and has 891 211 rows plus 366 columns. 
‘customers.csv` provides demographics data for customers of a mail-order company, it has 191,455 rows and 369 features columns, ‘mailout_train.csv` 
provides demographics data for individuals who were targets of a marketing campaign with 42 982 rows and 367 columns. 
‘mailout_test.csv’ provides the demographics data for individuals who were targets of a marketing campaign with 42,833 rows and 366 feature 
Lastly 'DIAS Attributes - Values 2017.xlsx' and 'DIAS Information Levels - Attributes 2017.xlsx' provide data about what the columns and the values mean.

#What kind of analysis was done?
First the data was analyzed using an unsupervised model, particularly K-means clustering that should predict whether customers of the mail order company 
fit into a specific cluster(s) of the general population. Next a superivised learning model was fitted to the data with a binary response (0 for not a 
customer and 1 for a customer) with the attempt of having a predictive model that could say whether or not a household would become a customer or not. 
Several algorithms were used in the machine learning model including gradient boost, random forest, ada boost, bag classifier,and logistic regression.
A pipeline was implemented with hyperparameters to optimize the model. 

#How did the models perform?
The unsupervised model worked very well. Plotting the variance vs. number of clusters showed that a good number of clusters to choose is about 8 and using
this value showed very clearly that the customers fall into three of the eight clusters with a high proportion and a low proportion in the others. This
suggests that given complete information about a household it could easily be ascertained what cluster they belong to and whether it is worth targeting them
for advertisement. 

Unfortunately the machine learning model did not fare very well and scored a very low roc-auc score. This was a surprise considering the clustering model 
worked so well it was easy to assume the maching learning model would too. It could be that the hyperparameters need more fine tuning or there could be 
some other unidentified issue. 

#A report for this project was published on 'Medium' a the following link: https://bryanchambers-25994.medium.com/customer-segmentation-for-bertelsmann-arvato-project-ce3edd722be4

