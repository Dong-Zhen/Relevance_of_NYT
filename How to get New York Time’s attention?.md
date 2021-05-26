# According to the U.S. Census, New York has a total population of  20,201,249. The New York Times has 5.26 million paid subscribers in the first quarter of 2021 according to statista.com. Only a small percentage of New York’s total population is subscribed to the New York Times. How can the New York Times increase their number of New York readers? 

While I do not know how many New Yorkers are subscribed to the New York Times, I do know that the New York Times has a New York column that targets New Yorkers. New York is known for its diverse population consisting of many different ethnic groups with varying income and education levels. I can help New York Times better understand the New York market so that they can personalized outreach campaigns to their intended market and increase readership. 

### Impact Hypothesis: By understanding the demographic, social, housing, and economic characteristics of New Yorkers, the New York Times can implement personalized outreach campaigns to target groups who are likely to subscribe in order to increase readership in the New York column.

The campaign is a success when the number of page views in the New York column is increased by 20% in four months.
The long term success measure is the New York column hitting a million daily readers

Constraints: Unable to target individuals of these groups directly. Need to target by location or through medias that cater to these groups. 
NYT Actions: Advertise to groups with higher likelihood of subscribing, Personalized emails to current subscribers, Produce and share relevant content to target groups

### Dataset: Location, Income, Industry, Age, Ethnicity, Education Data from American Community Survey 5-Year (2009-2019)

### Preliminary Analysis: 

Goal: Explore the dataset to understand how diverse New York is and the potential target markets by gender, income, education, industry. These features could be key indicators of who is likely to subscribe.

- How educated are New Yorkers?
- What are the age groups of New Yorkers?
- What are their income levels?
- Employed or unemployed?
- What industry?
- What are their ethnicities?

![Educated NYS Females](https://github.com/Dong-Zhen/Relevance_of_NYT/blob/main/Tableau/Female%20Education%20LVL.jpg)
![Educated NYS Males](https://github.com/Dong-Zhen/Relevance_of_NYT/blob/main/Tableau/Male%20Education%20LVL.jpg)

There is a large market of educated Females and Males in New York State.

![NYS Females Age](https://github.com/Dong-Zhen/Relevance_of_NYT/blob/main/Tableau/NYS%20Female%20Age.jpg)
![NYS Males Age](https://github.com/Dong-Zhen/Relevance_of_NYT/blob/main/Tableau/NYS%20Male%20Age.jpg)

Many New Yorkers are within the ages of 18-60.  

### Solution Path 1:

Interpretive 
Logistic regression to see what features inform of a likely subscriber 
The New York Times should see an increase in subscribers as they focus on New Yorkers who are likely to subscribe
The model is predicting accurately on a test set

### Solution Path 2: 

Unsupervised clustering to group New Yorkers into likely to subscribe and unlikely to subscribe groups and to better cater to target groups. 
The New York Times should see an increase in subscribers as they focus on relevant messaging to potential subscribers
The clustering is accurately grouping New Yorkers and identifying target groups for New York Times to promote relevant messages
