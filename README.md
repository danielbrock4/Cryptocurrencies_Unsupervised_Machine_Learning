# Cryptocurrencies & Unsupervised Machine Learning

## Resources

- **Data Source:** 
  - [crypto_data.csv](crypto_data.csv)
- **Software:** Python, Pandas, Hvplot, Plotly, Sklearn

## Challenge Project Overview 

Using Sklearn, Python, & Plotly, I analyzed a dataset of cryptocurrencies with unsupervised machine learning algorithms to spot any trends that would make a client want to invest in them. Since Ethereum and Bitcoin have already exploded in value, there is great interest in finding the next big project among all the alternative coins. That said, I will be using unsupervised machine learning to see if we can spot any trends resulting in altcoin opportunities. 

## Challange Project Analysis

#### Step 1: Preprocessing the Data for PCA 

I began by preprocessing the dataset provided so that the machine learning algorithm would run correctly. The preprocessing process started by uploading the CSV dataset, filtering only tradable currencies, dropping null values, double-checking for missing values, keeping mined coins only, and numerically encoding categorical columns using the pandas.get_dummies method, and scaling the data using the StandardScaler() method.

#### Step 2: Reducing Data Dimensions Using PCA

Next, using Principal Component Analysis (PCA), I reduced the dimension of 98 scaled columns to only three principal component columns.
![Fig1]/(images/fig1.jpeg)

#### Step 3: Clustering Crytocurrencies Using K-Means

To see how many clusters (k) I could divide the cryptos in, I created an elbow curve to identify the best number of clusters. 
![Fig2]/(images/fig2.jpeg)

The ideal amount of clusters is were line graph starts to take a large, noticable pivot on the line graph. As it can be seen, the optimal result was 4 clusters. So, I then proceeded with the KMeans analysis to fit the pca dataframe and predict the clustering. The product was this clustered_df with a 'Class' column that showed the predictions to which group it belonged to.

![Fig3]/(images/fig3.jpeg)

#### Step 4: Visualizing Cryptocurrencies Results

To better interpet the data, I created visuals to beter understand the results. The 3D scatter plot located each clustered crypto in relation to the 3 principal components created on the PCA. As it is seen, there are 3 major groups and one outlier (which can be seen in yellow).

![Fig4]/(images/fig4.jpeg)

When plotting clustered cryptos by total supply and mined coins, there are two, noticable outliers. The first outlier, BitTorrent Crypto, has a large supply of and a lot of mined coins (BitTorrent Crypto) and another one with a lot of supply but not too many coins mined (TurtleCoin).


## Challange Project Summary

#### Three Recommendations for Addressing Disparities Among City Type

1) Decrease Fares in Rural and Suburban Areas To Encourage More Riders 
2) Shift Drivers from Urban Areas to Suburban Areas to Capture The 2nd Biggest Market 
3) Decrease Drivers in Urban Areas to Increase Market Demand to Drive Up Fares 

