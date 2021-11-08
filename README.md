**Quotations indicate the career success of public figures**

**Abstract:**

In general, more quotations indicate more popularity or at least more exposure to the public. This could be vital for the careers of public figures, including politicians, movie stars, or even athletics. We aim to quantify the level of exposure by extracting the relevant number of quotations from Quotbank and incorporating the reading statistics of the source news. This enables us to examine how the level of exposure of certain public figures change over time by comparing the quotation data before or after their major career events, such as political election, movie casting. We shall thereby explore the relationship between the exposure in news articles and the careers of politicians or celebrities. Utilizing the discovered relationship, we also hope to build a model using the quotation data to predict the future career advancement of public figures.
	
**Proposed Questions:**	
The first major goal is to examine the relationship between quotations and career success. We will put our focus on political figures and movie stars. For political figures, we hypothesize that more quotation and exposure to the public enhances their probability of winning in elections. We will look at the quotation data of candidates of senators and congressmen before the election happened and examine whether the more quoted candidates won more elections. For movie stars, we propose the similar hypothesize that more quotations help them to get more offers in good movies. For each actor, we plan to look at the total budgets of the movies he or she participated in each year. By comparing this budget data with quotations, we may test whether an increase in the budgets of participated movies follow an increase in quotations.

(**TO DO: Add explanation of how good the Quotebank covers the publishers after data preprocessing)**

However, we are also aware that quotations in different publishers have different impact on career. For example, a quotation in New York Times surely boosts the career more than a quotation in local tabloid. Instead of directly counting the quotation number, we will try to find corresponding reading statistics of the publishers and compute a popularity index based on the reading statistics. We will quantify the level of exposure by weighing the quotations by popularity indices and then compare the level of exposures to the career of public figures.

Additionally, we notice that there are two major types of quotations for any chosen public figure: the quotations said by the figure, or the quotations by others but mentioning the public figures. These two types of quotations may have different impacts on their careers. Therefore, after examining all quotations together, we plan to examine the two types of quotations separately and exaplore how they respectively affect the careers of public figures.

Moreover, we hypothesize that there may be different types of exposure increase for each public figure. Some politicians may gain popularity through years of accumulating fame, while some others may gain overnight fame through some accidents or sponsorships from other powerful people. We generate time-series quotation data to explore how the quotations of different figures change over time. We can then cluster these data to see if we can identify different types of quotation increase.

After exploring the relationship between quotation data and career success, we hope to build a model predicting future career advancements using the quotation data. (**TO DO: add details for training model)**

Finally, we also want to further explore two additional aspects of quotations. First, we are interested in finding a sentiment analysis model to analyze the support rate of a politician when they are mentioned in quotations said by others.We may further examine whether this support rate by others' quotations can reflect their final election results. Second, we are interested in looking at how the speech style in the quotations made by a politician affect the success odds. This question is inspired by the U.S. 2016 election, after which many republican politicians adopted the speech styles of Donald Trump. We want to examine whether the more coarse speech style (quantified by vocubulary, grammar use, sentence lengths) actually helps their political career. 

The six specific questions we want to answer are listed below:

1. Does Quotation number/exposure level affect election results or movie casting?
2. Do the two types of quotations (mentioned in quotations by others or the quotation directly said by the public figure) impact the careers differently?
3. Are there different types of quotations increase? For example, a sudden spike increase is different from a gradual increase.
4. Can we build a model using the quotation data to predict election results or furture moviw casting?
5. When examining the politicians mentioned in quotations by others, can we obtain a rough support rate based on sentiment analysis?
6. After 2016, does a more coarse speech styles improves odds of success?

**Additional dataset:**
1. Election results (House and Senate): https://electionlab.mit.edu/data	
2. Movie statistics: https://www.kaggle.com/rounakbanik/the-movies-dataset
3. Dataset for reading statistics?

**Methods:**
1. Get politician dataset (2015-), clean the name format, find quotations in Quotebank, both being quoted and as most possible speaker
2. Obtain the time series quotation/exposure data, with major event (election) marked
3. Train a machine learning model to predict result based on cadidates quotation/exposure data
4. Find a NLP model to determine the attitude of quotations toward the public figure mentioned in the quote
5. Analyze the vocabulary and sentence length of quotations said by candidate, before 2016 and after.



 
