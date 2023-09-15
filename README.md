# Twitter Sentiment Analysis

**Authors**: JF Roberts, Aung Is & Michael Romanski

<p align="center">
  <img width="800" height="300" src="images/Holywood.jpeg">
</p>

## Overview

Our data analytics firm, Flatiron Analytics has been hired by [SXSW](https://www.sxsw.com/) to perform sentiment analysis on tweets from the festival. This project analyses a data set that was crowdsourced by festival goers to assess positive or negative emotion towards both Apple and Google products. Based on our analysis results, we will make recommendations on which product brand has the most positive association amongst festival goers.

## Business Understanding

SXSW wants to develop a new app for their festival and are deciding whether to deploy it on the Apple Store or Google Play Store. Flatiron Analytics has been tasked with developing a predictive model to accurately identify whether a given tweet displays “positive”, “negative” or “neutral” emotion towards Apple and Google devices. Our analysis will provide SXSW with a clear direction on which Store to deploy their new app as well as how to utilize our predictive models for future festivals.
 

## The Data

<p align="center">
  <img width="800" height="300" src="images/d90etr2uv2t9idnbcshcl9eh3p-e60d36ec5ba6ce6543b246ef0041c504.png">
</p>

The data we used for our analysis was pulled from [Data World](https://data.world/crowdflower/brands-and-product-emotions) and includes 8,700 tweets from the 2011 SXSW festival. Sentiments each tweet was crow sourced where:

“The crowd was asked if the tweet expressed positive, negative, or no emotion towards a brand and/or product.”

The data set includes information about the text of each tweet, the product the tweet is directed at and the emotion towards that product.


## Data Processing.

An important step in any NLP project is to process the text, essentially widling it down to its key components. We achieved this by dropping irrelevant characters that are often found in tweets such as hashtags ‘#’, the ‘@‘ symbol as well as any numbers. 

There was an evident class imbalance where over 60% of our tweets were identified as “neutral” sentiments. After further analysis of these neutral tweets we also noticed that many of them were mis-represented as such and would have been more accurately identified as positive or negative sentiments. As a result, we dropped the neutral sentiments all together.


![img](images/pr_table.png)

## Recommendations 

1. **Apple over Google** - 

![img](images/)

2. **Use our predictive model to classify sentiments from future festivals** - 

![img](images/)

3. **Compare our predictive model to the crowd-sourced approach** - 

![img]()

## Next Steps

1. We would like source more reliable data as well as a larger data set. Hundreds of thousands of people attend the SXSW festival therefore a larger and more representative data set would help our predictive model.

2. As noted above, many of our “neutral” sentiments were mis-represented. We would like to conduct further analysis to better classify the neutral class. By doing so, we could develop a reliable multi-class predictive model rather than just a binary model.

3. Lastly, to get even more granular, we noticed that some tweets displayed both positive and negative sentiments towards the respective brands. Much like for the mis-represented “neutral” tweets, we would like develop a more accurate way to handle these tweets.

## Repository Structure

```
├── data
├── notebook.ipynb
├── working_notebooks
├── images
├── .gitignore
├── README.md
└── presentation.pdf
```
