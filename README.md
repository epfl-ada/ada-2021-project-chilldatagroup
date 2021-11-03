Abstract:
In general, more quotations extracted from news articles indicate more popularity or at least more exposure to the public. This could be vital for the careers of public figures, including politicians, movie stars, or even athletics. We can quantify the level of exposure by extracting the relevant number of quotations from Quotbank and incorporating the reading statistics of the source news. We can then examine how the level of exposure of certain public figures change over time and compare the time-series data to their major career events, such as political election, movie casting. We shall thereby explore the relationship between the exposure in news articles and the careers of politicians or celebrities. In addition, we may also train a model using the exposure level to predict the election results.
	
Proposed Questions:	
1. Does Quotation number/exposure level affect election results or maybe movie?
2. Are there different shapes/situations of quotations increase? Are there sudden spikes?
3. Are there differences between number Quoted by others v.s. number of own quotation?
4. Can we build a prediction model of election result? Movie career? Sports result?
5. When quoted by others, can we obtain a feel of support rate based on sentiment analysis?
6. After 2016, does exposure of vocabulary/shorter sentences improves odds of success?

Additional dataset:
1. Election results (House and Senate): https://electionlab.mit.edu/data	
2. Movie statistics: https://www.kaggle.com/rounakbanik/the-movies-dataset
3. Dataset for reading statistics?

Methods:
1. Get politician dataset (2015-), clean the name format, find quotations in Quotebank, both quoted and as most possible speaker
2. Obtain the time series quotation/exposure data, with major event (election) marked


To ask on Friday:
•	Data size: shall we just explicitly say the size?
•	What’s in the data: mathematical details in the Notebook? Jupyter or readme?
 
