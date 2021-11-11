**Quotations indicate the career success of public figures**

**Abstract:**

In general, more quotations indicate more popularity or at least more exposure to the public. This could be vital for the careers of public figures, especially politicians. We aim to quantify the level of exposure by extracting the number of quotations from Quotbank and incorporating the reading statistics of the source media. This enables us to examine how the level of exposure of certain public figures change over time by comparing the quotation data before or after their major career events, such as the political election. We shall thereby explore the relationship between the exposure in news articles and the careers of public figures. Utilizing the discovered relationship, we also hope to build a model using the quotation data to predict the future career advancement of public figures.
	
**Proposed Questions:**	
Based on our central interests in the relationship between the exposure in news articles and the careers of public figures. We choose to focus on how quotations of politicians correlate with the election results. Specifically, we propose four major questions.

1. The first question is whether politicians with more exposure to the public have better election results. We will look at the quotation data of candidates of senators and congressmen before the election happened and examine whether the more quoted candidates gained more votes. Meanwhile, we are also aware that quotations in different media offer different exposure level, thus having different impact on career. For example, a quotation in New York Times surely boosts the career more than a quotation in a local tabloid. We will quantify the exposure level by combining the quotations and the popularities of source media.

2. We noticed that there are two types of quotations for any public figure: the figure is the speaker of the quotations, or the quotations are said by others but the content includes the public figures. Therefore, we plan to examine whether the two types of quotations have different correlations to the election results of politicians.

3. We hypothesize that different politicians gain public exposure in different ways. Some politicians may gain popularity through years of accumulating fame, while some others may gain overnight fame through some accidents or sponsorships from other powerful people. We examine how the exposure level of each politicians change over time, and whether there are different types of exposure level changes.

4. After exploring the relationship between quotation data and career success, we hope to build a model predicting the results using the quotation data. 

The above four questions are the central questions for us to explore the relationship between quotation data and political elections. Finally, if we have time, we also want to further explore two additional questions addressing quotations and political elections. 

5. When examining the politicians mentioned in quotations said by others (the second type of quotations in question 2), we will try to find the proper sentiment analysis model to attitude (positive or negative) of the speaker toward the mentioned politicians. We want to test whether the attitude can reflect the support rate.

6. After 2016 election, many republican politicians adopted the speech styles of Donald Trump. We want to examine whether the more coarse speech style (simpler vocubulary and shorter sentence lengths) actually helps their political career. 

**Additional dataset:**
1. The senate election result by MIT Election Data and Science Lab[1]. It contains the election information of each candidate. We use the dataset to get the identity, party affiliation, and resulting votes of each candidate.
2. The presidential election result by MIT Election Data and Science Lab[2]. It contains the election information of each candidate in each states. We use the dataset to get the how much support each party get in 2016 and 2020 election. The support rate of each party in each state is used as features in our prediction model (Q4).

**Methods:**
1. Get politician dataset (2015-), clean the name format, find quotations in Quotebank, both being quoted and as most possible speaker
2. Obtain the time series quotation/exposure data, with major event (election) marked
3. Train a machine learning model to predict result based on cadidates quotation/exposure data
4. Find a NLP model to determine the attitude of quotations toward the public figure mentioned in the quote
5. Analyze the vocabulary and sentence length of quotations said by candidate, before 2016 and after.

**Internal Milestones and Proposed Timeline**

**Questions for TA**


**Reference**:
[1]MIT Election Data and Science Lab, 2017, "U.S. Senate 1976–2020", https://doi.org/10.7910/DVN/PEJ5QU, Harvard Dataverse, V5.

[2]MIT Election Data and Science Lab, 2017, "U.S. President 1976–2020", https://doi.org/10.7910/DVN/42MVDX, Harvard Dataverse, V6.
