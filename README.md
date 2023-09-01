# Credit-Card-Fraud-Neural-Network
This is a neural network to find Credit Card fraud, made using a training set from Kaagle, found here: (https://www.kaggle.com/datasets/dhanushnarayananr/credit-card-fraud?resource=download)

The tools used in this notebook include: TensorFlow, Keras, Sklearn, Matplotlib, and Numpy

This repository has a jupyter notebook called Credit Card Fraud, which can make and save the model. However, the training data must first be downloaded and can be found in the link to Kaagle.

The training data has 8 features, distance_from_home, distance_from_last_transaction, ratio_to_median_purchase_price, repeat_retailer	used_chip, used_pin_number, online_order, and fraud.

The neural network currently has three layers. The first and second layers have 64 and 32 nodes respectively, and use ReLU activation. The third layer has one node and uses sigmoid activation as this is a binary classification problem. The model is compiled using the Adam optimizer, the binary cross-entropy loss function, and the accuracy metric. Below is an image of the output of the .summary() function.

![alt text](https://github.com/RevanthKrishna2004/Credit-Card-Fraud-Neural-Network/blob/main/summary.png?raw=true)



I have attached two models, one that has been trained with 10 iterations (ccf_model_one.keras), and one that has been trained with 100 iterations (ccf_model_hundred.keras).

The ccf_model_one.keras has an accuracy of 99.6% and an F1 score of 84.6%.
The ccf_model_hundred.keras has an accuracy of 99.7% and an F1 score of 98.6%.

Below is the confusion matrix of the ccf_model_hundred.keras model.
![alt text](https://github.com/RevanthKrishna2004/Credit-Card-Fraud-Neural-Network/blob/main/table-chart.png?raw=true)

This graph shows the total loss over ten training iterations for the model I have included. The notebook also contains a block of code to make this graph.

![alt text](https://github.com/RevanthKrishna2004/Credit-Card-Fraud-Neural-Network/blob/main/graph.png?raw=true)
