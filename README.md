# Cryptocurrencies

## Overview
This unsupervised machine learning project analyzes cryptocurrency data to classify trading markets for investments. Since there is no known output, unsupervised machine learning was used to cluster the cryptocurrencies. 

## Resources
- Datasource: [CryptoCompare](https://min-api.cryptocompare.com/data/all/coinlist)
- Python
- Pandas
- HV Plot
- Plotly Express
- SKLearn

### Processing Data
Reviewing raw data, filtering for coins that are actively trading, removing null values, filtering for coins that have been mined and dropping unnecessary data columns for ML. Creating Variables for text features(Algorithm and ProofType) with get_dummies() and using the StandardScale to standardize the features.

### Reducing Data Dimensions Using PCA
Reducing the dimensions to 3 principal components.

### Clustering Cryptocurrencies Using K-means
Creating an elbow curve with hvPlot to find the best value for K.
![Elbow_curve](Images/01_ElbowCurve.png).

K=4. Making predictions of the K clusters.

### Visualizing Cryptocurrencies
3D Scatter Plot of all three clusters with the Coin Name and Algorithm 
![3D_Scatter](Images/02_3DPlot.png)
Created a table with currencies
![Table](Images/03_Table.png)

2D Scatter Plot of total Coins Mined vs. Total Coin supply by class.
![2D_Scatter](Images/04_Scatter.png)
