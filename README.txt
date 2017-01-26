NYC Connect - Taxi Demand Prediction System
Khyati Savakia
-------------------------------------------------------------------------------
This project includes implementation of K-Means, Naive Bayes and Logistic Regression
algorithms to predict areas with high taxi demand and also the surge charge that is 
likely to be imposed.
---------------------------------------------------------------------------------
Please find the below instructions to run the project on Hadoop cluster:

NAIVE BAYES & K-MEANS

1. Instruction to run on dsba-hadoop cluster:

$ spark-submiy NaiveBayes.py <input file name> <"Timeslot"> <"Day”>

For example: $ spark-submit NaiveBayes.py green_tripdata_2016-06.csv "3" "Wednesday"

LOGISTIC REGRESSION

1. Instruction to run on dsba-hadoop cluster:
$ spark-submit PredictionUsingLogisticReg.py  <input file name> <output file name>

For example:$ spark-submit PredictionUsingLogisticReg.py Testing_Dataset_taxi.csv /home/output

Web-Page for Project Report: http://webpages.uncc.edu/nbhirud/
Data set for the project is uploaded on the Dropbox:
green_tripdata_2016-06.csv: https://drive.google.com/file/d/0BwwRPutczcp1QzhaV01YRTg2MVE/view?usp=sharing
Testing_Dataset_taxi.csv: https://drive.google.com/file/d/0BwwRPutczcp1THJhV1Y3bE02OFU/view?usp=sharing

File: Training_Model_Logistic.py contains the code used for training the model to get weighted with highest accuracy.
File: NaiveBayes_Kmeans_Test_Train.py contains the code for training and testing our model with 80% and 20% data.







