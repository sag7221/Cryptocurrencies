# Cryptocurrencies

## Purpose
Unsupervised machine learning is for understanding data, patterns from a given dataset. In this project, a prominent investment bank is looking at offering a cryptocurrency investment portfolio for customers.
But given the vast universe of cryptocurrencies we have been asked to create a report to understand cryptocurrencies in today's trading market and classification of this data to make it easier for customers to understand.

### Details with Steps
Given the data, we first had to process this data to make it easier to train our models. As it is data that we were still trying to udnerstand, we figured it is best to implement unsupervised machine learning techniques as follows:
1. We first read the csv into a DataFrame and processed data to remove nulls, unwanted columns and filtered data to retrieve only those currencies that have been mined
2. We scaled data to implement Dimensionality reduction using PCA
3. We tried to create an Elbow Curve to find out optimal clusters that our data can be classified into
4. After this we created visualizations to see how data has been classified.
5. Next we wanted to figure out the supply and demand situation for these currencies, for this we again scaled columns "TotalCoinsMined" and "TotalCoinSupply" to create a visualization.
6. We then created a visualization for this.

### Results And Analysis
* Once we had our data set ready for PCa, we first scaled it and then implemented PCA and plotted to find the optimum number of clusters. Below are our results:\
![Elbow Curve](https://github.com/sag7221/Cryptocurrencies/blob/main/images/Elbow_Curve.png)

* From above picture, i estimated optimal K clusters is 4 and ran a KMeans model for 4 clusters.\
Below is how KMeans clusters look like:\
![KMeans Clusters](https://github.com/sag7221/Cryptocurrencies/blob/main/images/KMeans_3D.png)

* I now also wanted to do further analysis and created a visualization of tradeable cryptocurrencies\
![Crypto Currencies](https://github.com/sag7221/Cryptocurrencies/blob/main/images/tradeable_cryptos.png)

* A total of 532 such tradeable crypto currencies exist in this dataset. I now scale the columns TotalCoins Mined and TotalCoins Supply to get an idea of status of these currencies. Scaling was done using MinMaxScaler\
![Scatter Plot](https://github.com/sag7221/Cryptocurrencies/blob/main/images/scatter_plot.png)






