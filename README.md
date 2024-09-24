# Objective
For the dataset of concrete_compressive_strength, I removed some data from superplasticizer column
We want to predict the accuracy of the ANN model in predicting the correct values of the superplasticizer.
We want to have the ANN model to interpolate those missing data with a meaningful data

# Illustration
1) Training: We train an linear ANN model on the dataset
2) Input features: Columns with complete data
3) Output Target: Columns with missing data
4) Testing: We predict the columns with missing data after training the model 
by entering the inputs features to the network
and let the model predict the output

# Model & Architecture
1) ANN DL Model
2) input layer:   8  -> relu -> 64 
3) Hidden Layer1: 64 -> relu -> 64
4) Hidden Layer2: 64 -> relu -> 10
5) Output Layer:  10 -> 1
6) Got better results without batchnorm
7) Normalize inputs using z-transform
8) Use of MSELoss because we predict a continuous number 


# Results
1) Accuracy: Got 99% accuracy for the prediction of the superplasticizer

# Conclusions:
1) Interpolations of missing data in datasets using DL models is working perfectly and can be used instead of dropping those rows with missing data from training.
