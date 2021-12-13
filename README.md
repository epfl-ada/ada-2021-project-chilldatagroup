**Can Quotations of Politicians Indicate Election Results?**

**Link to Data Story Website:** https://zihan-wu.github.io/SenateQuotationWeb/

**Abstract:**

In general, more quotations in news articles indicate more popularity or at least more exposure to the public. Quotations could thereby be vital for the successful careers of politicians. On the other hand, successful politicians are also more frequently quoted in news. Thus, the career of politicians may be highly correlated with quotations. The recent release of QuoteBank, a corpus of quotations from news, can be useful in extracting the quotations of politicians. In this project, we will focus on the U.S. Senate elections. First, combining the quotations and election results, we want to answer whether more quoted senate election candidates tend to have better election results. Then, we aim to examine if quotations can be an efficient predictor of election results. Furthermore, quotations can either praise or criticize the politicians. Recent advancements in language sentiment analysis enable us to get attitudes toward quoted candidates. We will explore how such attitudes correlated with election results.
	
**Proposed Questions:**	

Based on our interests in the relationship between quotations in news articles and the careers of politicians, we propose five specific questions.

1. The first question is whether politicians with more quotes have better election results. Meanwhile, we are also aware that quotations in different media offer different exposure levels, thus having a different impact on careers. For example, a quotation in New York Times shows more popularity than a quotation in a local tabloid. We will weigh the quotes by the website views of source media.

2. For any politician, we noticed that there are two types of relevant quotations: the politician is the speaker of the quotations, or the quotations are said by others but the content includes the politician. Therefore, we plan to examine whether the two types of quotations have different correlations to the election results of politicians.

3. We hypothesize that different politicians gain public exposure in different ways. Some politicians may gain popularity through years of accumulating fame, while some others may gain overnight fame through some accidents or sponsorships from other powerful people. We examine how the exposure level of each politician change over time, and whether there are different types of exposure-gaining process.

4. After exploring the relationship between quotation data and career success, we hope to build a model predicting the election results using quotation data.

5. When examining the politicians mentioned in the quotations said by others (the second type of quotations in question 2), we will try to find the proper sentiment analysis model to obtain the attitude (positive or negative) of the speaker toward the mentioned politicians. We want to test whether the attitude can reflect the support rate.

**Additional dataset:**

1. The senate election result by MIT Election Data and Science Lab[1]. It contains the election information of each candidate. We use the dataset to get the identity, party affiliation, and resulting votes of each candidate.

2. The statewide presidential election result by MIT Election Data and Science Lab[2]. It contains the election information of each candidate in each state. We use the dataset to get how much support each party gets in the 2016 and 2020 elections. The support rate of each party in each state is used as a feature in our prediction model (Q4).


**Methods:**

To answer questions 1 and 2, we calculate how many quotations are related to a candidate before the election. We use Pearson correlation to examine the relationship between the numbers of two types of quotations and the resulting vote rate. To get the exposure level of each quotation, we weigh the quotation by the scaled readership of the source media.

To answer questions 3 and 4, we calculate the number of quotations of each candidate each day. This generates time-series data capturing the changes of quotation numbers. We will discretize this time series data by quotations in each month. We plan to cluster these discretized data to identify different types of the exposure-gaining process in question 3. For the prediction model in question 4, we will use time-series data (which is a high dimensional vector), the affiliated party, and the party's performance in the recent election (an indicator of the state's ideology) as features in training and prediction.

For question 5, we plan to find a sentiment analysis model to determine whether the speaker of quotes supports the candidate mentioned in the quotes. We will calculate the support rate of each candidate in the quotes, and compute its correlation to the resulting vote rate.

**Internal Milestones and Proposed Timeline**

We plan 5 milestones, each accomplished in a week:
1. By Nov.19th: Collected the readership of the frequently appearing source media 
2. By Nov.26th: Finished homework2. Found the appropriate sentiment analysis model.
3. By Dec.3rd: Calculated the exposure level of quotations. Extracted the sentiments.
4. By Dec.12th: Clustered the quotation data and examined different exposure gaining process.
5. By Dec.17th: Built the prediction model and wrote the final report.

**Contributions**

Zihan Wu: Load quotations said by candidates, found election result data, collected website views of media, wrote README.md report.

Yinhao Wang:

Yihang Chen:


**Reference**:

[1]MIT Election Data and Science Lab, 2017, "U.S. Senate 1976–2020", https://doi.org/10.7910/DVN/PEJ5QU, Harvard Dataverse, V5.

[2]MIT Election Data and Science Lab, 2017, "U.S. President 1976–2020", https://doi.org/10.7910/DVN/42MVDX, Harvard Dataverse, V6.
