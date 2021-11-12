**Quotations indicate the career success of public figures**

**Abstract:**

In general, more quotations indicate more popularity or at least more exposure to the public. Thus, quotations could be vital for the careers of public figures, especially politicians. We aim to quantify the level of exposure by extracting the number of quotations from Quotbank and incorporating the readership (how many people read) of the source media. This enables us to examine how the level of exposure of certain public figures changes over time and to compare the quotation data before or after their major career events, such as the political election. We shall thereby explore the relationship between exposure in news articles and the careers of public figures. Utilizing the discovered relationship, we also hope to build a model using the quotation data to predict the future career advancement of public figures.
	
**Proposed Questions:**	

Based on our interests in the relationship between exposure in news articles and the careers of public figures, we choose to focus on how quotations of politicians correlate with the election results. Specifically, we propose four major questions.

1. The first question is whether politicians with more quotes have better election results. Meanwhile, we are also aware that quotations in different media offer different exposure levels, thus having a different impact on careers. For example, a quotation in New York Times surely boosts the career more than a quotation in a local tabloid. We will weigh the quotes by the readership of source media.

2. For any politician, we noticed that there are two types of relevant quotations: the politician is the speaker of the quotations, or the quotations are said by others but the content includes the politician. Therefore, we plan to examine whether the two types of quotations have different correlations to the election results of politicians.

3. We hypothesize that different politicians gain public exposure in different ways. Some politicians may gain popularity through years of accumulating fame, while some others may gain overnight fame through some accidents or sponsorships from other powerful people. We examine how the exposure level of each politician change over time, and whether there are different types of exposure-gaining process.

4. After exploring the relationship between quotation data and career success, we hope to build a model predicting the election results using the quotation data.

Besides the four central questions, we also want to further explore two additional questions addressing quotations and political elections.

5. When examining the politicians mentioned in the quotations said by others (the second type of quotations in question 2), we will try to find the proper sentiment analysis model to obtain the attitude (positive or negative) of the speaker toward the mentioned politicians. We want to test whether the attitude can reflect the support rate.

6. After the 2016 election, many republican politicians adopted the speech styles of Donald Trump. We want to examine whether the more coarse speech style (simpler vocabulary and shorter sentence lengths) helps their political careers after 2016.

**Additional dataset:**

1. The senate election result by MIT Election Data and Science Lab[1]. It contains the election information of each candidate. We use the dataset to get the identity, party affiliation, and resulting votes of each candidate.

2. The statewide presidential election result by MIT Election Data and Science Lab[2]. It contains the election information of each candidate in each state. We use the dataset to get how much support each party gets in the 2016 and 2020 elections. The support rate of each party in each state is used as a feature in our prediction model (Q4).


**Methods:**

To answer questions 1 and 2, we calculate how many quotations are related to a candidate before the election. We use Pearson correlation to examine the relationship between the numbers of two types of quotations and the resulting vote rate. To get the exposure level of each quotation, we weigh the quotation by the scaled readership of the source media.

To answer questions 3 and 4, we calculate the number of quotations of each candidate each day. This generates time-series data capturing the changes of quotation numbers. We plan to cluster these time-series data to identify different types of the exposure-gaining process in question 3. For the prediction model in question 4, we will use time-series data (which is a high dimensional vector), the affiliated party, and the party's performance in the recent election (an indicator of the state's ideology) as features in training and prediction.

For question 5, we plan to find a sentiment analysis model to determine whether the speaker of quotes supports the candidate mentioned in the quotes. We will calculate the support rate of each candidate in the quotes, and compute its correlation to the resulting vote rate.

For question 6, we will analyze the language complexity in quotations said by candidates. We will compute the correlation between some complexity criteria (sentence length, vocabulary, grammar error, etc.) and the final vote rate. We plan to check whether the correlation changes before and after the 2016 election.

**Internal Milestones and Proposed Timeline**

We plan 5 milestones, each accomplished in a week:
1. By Nov.19th: Collect the readership of the frequently appearing source media, calculate the exposure level of quotations, and complete the analysis for question 3.
2. By Nov.26th: Build the prediction model and evaluate its performance.
3. By Dec.3rd: Find the appropriate sentiment analysis model.
4. By Dec.10th: Complete the analysis for questions 5 and 6.
5. By Dec.17th: Finish writing the final report and cleaning the code.

**Questions for TA**

1. For the prediction model, we will consider both the time series quotation data and other features like party affiliation. The simplest way to combine them is just to concatenate. Do you have suggestions on how to combine these features in a smarter way?
2. When weighing the quotations by readership, we find it difficult to extract media readership information just from QuoteBank, because it only gives an url. For now, we decide to manually look up the readership of the most frequently appearing media. For the rest media, we assign a sampled mean to their readership (more details in the notebook). Do you have suggestions on this method?


**Reference**:

[1]MIT Election Data and Science Lab, 2017, "U.S. Senate 1976–2020", https://doi.org/10.7910/DVN/PEJ5QU, Harvard Dataverse, V5.

[2]MIT Election Data and Science Lab, 2017, "U.S. President 1976–2020", https://doi.org/10.7910/DVN/42MVDX, Harvard Dataverse, V6.
