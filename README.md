# Health-insurance-cross-sell-prediction

<h3>Problem Statement</h3>
An Insurance company that provides health insurance to its customers is planning on expanding their products and the product team is analyzing the possibility of offering policyholders a new product: Vehicle insurance.

Just like medical insurance, there is vehicle insurance where every year customer needs to pay a premium of certain amount to insurance provider company so that in case of unfortunate accident by the vehicle, the insurance provider company will provide a compensation (called ‘sum assured’) to the customer.

Building a model to predict whether a customer would be interested in Vehicle Insurance is extremely helpful for the company because it can then accordingly plan its communication strategy to reach out to those customers and optimise its business model and revenue.

<h3>Project Summary</h3>
<h5>Data:</h5>

The given data is a survey dataset which contains customer information such as their age , vehicle age,vehicle damage , previous insurance etc and their response for wheter they are intrested in buying vehicle insurance . This is a dataset for binary classification and contained data for 381109 records which has total of 11 columns.


<h5>Preprocessing of data and EDA:</h5>

Initially we started with loading the dataset, checked for duplicate values, nan values. Formed some hypothesis about the data.

Plotted distribution plots and box plots for numerical variables. Following up did exploratory data analysis and studied the independent variables its distribution and its impact on target output and did hypothesis testing by performing EDA.

After plotting the heatmap we donot see multicolinearity, as no two variables were highly correlated with each each other. The dependent variable(Response) is postively correlated with all other variables except previously insured variable.


<h5>Feature engineering and Model Training:</h5>

In feature engineering we treated the categorical columns and one hot encoded them. The data set was highly imbalanced dataset so, Data imbalance was treated by synthetic oversampling(SMOTE) technique. Followed by model training in which data was divided in train and testing set and was also standarzised.


<h3>ML ALgorithms implemented:</h3>


1.Logistic Regression

2.KNN Classifier

3.Decission Tree

4.Random Forest classifier

5.XGB Classifier


<h3>Conclusion:</h3>

1.All the models have given almost similar accuracy scores. We have got best accuracy score for Random forest model, but since this was a classification model for a highly imbalanced dataset accuracy was not a good metric to judge the model performance. So, precision, recall,f1 and ROC_AUC scores were also studied and Random Forest model gave the best results.

2.Random forest Regressor have given the highest accuracy score of 0.898619 and 0.900524 Precision, 0.896224 Recall, 0.898369 F1 score and 0.898629 ROC_AUC score.Hence, Random forest is chosen as best performing model.
