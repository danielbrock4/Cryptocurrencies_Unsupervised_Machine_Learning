# Cryptocurrencies & Unsupervised Machine Learning

## Resources

- **Data Source:** 
  - [crypto_data.csv](crypto_data.csv)
- **Software:** Python, Pandas, Hvplot, Plotly, Sklearn

## Challenge Project Overview 

Using Sklearn, Python, & Plotly, I analyzed a dataset of cryptocurrencies with unsupervised machine learning algorithms to spot any trends that would make a client want to invest in them. Since Ethereum and Bitcoin have already exploded in value, there is great interest in finding the next big project among all the alternative coins. That said, I will be using unsupervised machine learning to see if we can spot any trends resulting in altcoin opportunities. 

## Challange Project Analysis

#### Step 1: Preprocessing the Data for PCA 

I began by preprocessing the dataset provided, so the maching algrothim would run correctly. The preprocessing process started by uploading the CSV dataset, filtering only tradable currencies, dropping null valuesm double checking for missing values, keeping mined-coins only, and numerically encoding categorical columns using the pandas.get_dummies method, and scaling the data using the StandardScaler() method, as well.

#### Step 2: Reducing Data Dimensions Using PCA

Next, using Principal Component Analysis (PCA) I reduced demension of 98 scaled columns to only 3 principal component columns.

**Analysis Results:**
  - Results Notebook: [PyBer_Challenge.ipynb](PyBer_Challenge.ipynb)
  - Differences In Ride-Sharing Data Among Different City Types
![Fig9](Analysis/Fig9.PNG)
  - Line Chart: 
![Fig8](Analysis/fig8.png)

## Challange Project Summary

#### Three Recommendations for Addressing Disparities Among City Type

1) Decrease Fares in Rural and Suburban Areas To Encourage More Riders 
2) Shift Drivers from Urban Areas to Suburban Areas to Capture The 2nd Biggest Market 
3) Decrease Drivers in Urban Areas to Increase Market Demand to Drive Up Fares 

