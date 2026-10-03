# predictive-power-of-imbalance

In this repository, we study the predictive power of the imbalance. The objective is to predict futur price movements using the imbalance. The data used in this project is about the Order Book of the asset **Total** and contains the volume of the Bid/Ask order book, the sign of the last 10 transaction, the normalized transaction volume. The target is then *diff(h)* which is the futur increase price for a given horizon *h*. 

# Linear Regression  :
We first use a linear Model that we fit to our data (imbalance, diff(h)). We then test the model using a R2 score 

# Neural Network : 
- We use a Neural Network as a more sofiscated model. For that we had to prepare the data for it by splitting the dataset between a training part and a testing part. We then normalized the data.

- For the Neural Network itself, we used a hidden layer of size 32 and a ReLU activated function. 

- We then test the performance of the NN on the test dataset using R2 metrics. 

# Results and Conclusion :
- The features used are very good explanotory and so predictive variable for futur prices movements. (in general r2 > 0.95)

- The NN outperforms the linear regression for large horizons h. 
