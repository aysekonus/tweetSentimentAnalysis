# Determining the correlation between the stock market and tweet volume using sentiment analysis

> Determining the relationship between the market value of the company and the public opinion of that company with the analysis of the data set, the sensitivity analysis of the companies with the time series in the chart and the reasoning of possible decreases and increases.

## Datasets
- [Tweets about the Top Companies from 2015 to 2020](https://www.kaggle.com/datasets/omermetinn/tweets-about-the-top-companies-from-2015-to-2020)
- [Values of Top NASDAQ Companies from 2010 to 2020](https://www.kaggle.com/datasets/omermetinn/values-of-top-nasdaq-copanies-from-2010-to-2020)

**The dataset on [“Tweets about the Top NASDAQ Companies from 2015 to 2020”](https://www.kaggle.com/datasets/omermetinn/tweets-about-the-top-companies-from-2015-to-2020) includes tweets about the companies covered by NASDAQ between 2015 and 2020. NASDAQ is recognized as the world's technology exchange. It is a stock market where the stocks of almost all companies that direct information technologies today, including world giant companies such as Apple, Google, IBM, Netflix, Amazon, Tesla, Microsoft, Facebook, Twitter, are traded.**

**This dataset was created to identify possible speculators and influencers in an exchange. The tweet ID includes information such as the author of the tweet, the date of posting, the text body of the tweet, and the number of comments, likes, and retweets of tweets that match the relevant company. With the analysis of the data set, it is aimed to determine the relationship between the market value of the company and the public of that company, to analyze the sensitivity of the companies with time series in the graph and to reason about possible decreases and increases.**

**Within the scope of the study, the Python programming language was used for the analysis of the data; Many libraries such as pandas, yfinance, matplotlib, seaborn, wordcloud, nltk have been used. Classification, clustering, regression methods were investigated and algorithm methods were examined, and the most suitable methods were selected and applied for the project. In this study, the relationship between Twitter and stock prices, which is one of the social media platforms, was tried to be revealed. For this purpose, the data sets were combined and passed through various pre-processing techniques, and sentiment analysis was performed on the data.**

## STATISTICAL ANALYSIS OF THE RELATIONSHIP BETWEEN TWEET VOLUME AND COMPANIES' SHARE TRADING VOLUME

**It was desired to learn whether the amount of tweets sent in line with the project affects the transaction volume of a particular company. This required comparing the effects of tweet volume the day before on the stock price of a particular company the next day. In this direction, all time series were shifted back by 1 point and the relationship between them was examined in the most efficient way. For this, the shift operator belonging to the pandas library is used. In order to examine the relationship between tweet volume and stock market trading volume, correlation analysis was performed and spearman statistics test was applied. In addition to the statistical test, the traded stock market volume and tweet volume are plotted on the same graph to visualize the data for an overview of the relationship between these 2 variables. An average of 30 days of examination was deemed sufficient to obtain a clearer visualization of the relationship between these two variables and to have a clearer understanding of the general trend, and the rolling operator, which also belongs to the pandas library, was used for this.**

### SPEARMAN CORRELATION STATISTICS TEST

> In line with the hypothesis, if the p-value of the Spearman correlation falls below the predetermined threshold of 0.05, the null hypothesis will be rejected and it will be concluded that there is sufficient evidence to conclude that there is a positive/negative correlation between the volume of stock traded and the volume of tweets.

**HYPOTHESIS:**
- **Null hypothesis:** There is no correlation (correlation) between tweet volume and traded stock volume.
- **Alternative hypothesis:** There is a correlation (correlation) between tweet volume and traded stock volume.

### SENTIMENT ANALYSIS

**Today, social media platforms such as twitter, facebook, instagram are used to obtain information and also to share information. Social media users provide information, share their feelings or present their ideas about a subject by sharing data in various ways such as text and pictures. Therefore, social media platforms are a rich source of data for text mining or opinion mining. Social media content includes not only information about the event, but also the emotions of the users who created them. Users' thoughts about a particular event are extracted through text analysis, and then emotions are predicted based on the analysis obtained. However, various text mining methods are used to discover information from the data here. One of them is sentiment analysis method. It is used to analyze whether the hidden feelings and thoughts in the texts are positive, neutral and negative. As a result of the operations performed in the analyzed data set, 2488 positive, 1501 neutral and 1276 negative tweets were obtained.**

<img width="367" alt="image" src="https://user-images.githubusercontent.com/68853621/174500095-2e9ca8bf-7421-4c9f-91d4-ee5c8577b9a9.png">

> NOT: Analyzes were carried out on positive and negative tweets.

### CONCLUSION
---

**It is seen that only 4 of the 10 most popular tweets examined have an impact on the stock market. In other words, tweet volume affects stock market trading volume by only 40%. As a result, it is seen that the tweets are 28% positive, 24% negative and 47% neutral. It has been observed that tweet volume and twitter have an effect on the stock market, but it is concluded that there is no certainty that it will increase or decrease stock prices even if a tweet is viral.**
