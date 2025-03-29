# Credit-Card-Fraud-Detection
EDA.ipynb file contains the code for Exploartory Data Analysis of the dataset.
CNNDIST.ipynb evaluates the dataset using CNN Model.
LSTMDIST.ipynb evaluates the dataset using LSTM Model.

When using machine learning techniques, feature selection (FS) is essential, especially when 
datasets have a large number of features that could impair model performance. Random Forest, a 
widely-used ensemble learning method, was employed for feature selection because of its ability 
to rank features based on their contribution to reducing impurity during tree-building. The dataset 
was split into 80% training and 20% testing for the purpose of evaluating the model. 
The most significant characteristics for predicting fraudulent transactions were identified by 
extracting and ranking feature importance scores after the model was trained on the training data. 
This process streamlined the dataset, improving model efficiency, interpretability, and reducing 
overfitting. Analysis revealed that location-based features such as zip, lat, lang, merch_lat, and 
merch_long were among the most significant predictors of fraudulent activity. The unix_time 
feature, representing the transaction time in Unix format, also emerged as a key predictor. 
To capture the spatial relationship between transaction and merchant locations, a new feature 
named distance was created. Using the latitude and longitude coordinates of both points, the 
great_circle function from the geopy library computed the distance in kilometers,offering insights 
into the physical proximity between transactions and merchant locations. 
