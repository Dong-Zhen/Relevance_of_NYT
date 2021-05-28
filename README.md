# Abstract

New York Times is a highly circulated American newspaper, 18th in the world and 3rd in the US, that focuses on delivering content that enriches their reader's lives and to make society more strong and just. Since New York Times started focusing on their digital platform and growing it to 5.6 million subscribers in the first quarter of 2021, there has been a drop in their print circulation especially in New York. In 2013 they were circulating an average of 1,926.8 daily print newspapers in New York and has dropped to an average of 374 daily print newspapers in 2021. There's an opportunity for them to attract New Yorkers to the digital version of their newspaper. By reaching out to New Yorkers, they can increase the daily readership of the New York column and improve page view and engagement metrics. Before New York Times can reach out, they have to understand the New York population. 

After analyzing data from the 5 year American Community Survey for 2009 - 2019, I learned that the majority of New York adults' education backgrounds fit New York Time's target market. However, the state is diverse in age, location, industry, and ethnicity, which requires New York Times to think about who to target. As a data scientist I can apply logistic regression on Census and subscriber data to help New York Times find out who is likely to be a subscriber and who is not. Through this model, the New York Times can come up with relevant marketing campaigns to target likely subscribers.


## Design

### Impact Hypothesis: By understanding the demographics and social characteristics of New Yorkers 25 and older, the New York Times can implement personalized outreach campaigns to target groups who are likely to subscribe in order to increase readership in the New York column.

### Additional Impacts:

- Readers read other columns as well, increasing the columns' engagement metrics
- Increase in subscribers 
- Advertisers pay more to reach specific groups

### Ways the Hypothesis Could Fail: 

- New Yorkers are not interested in the New York column's content
- Likely to subscribe does not equal higher readership, target group might subscribe to other newspapers as well

### Solution Path: Build a logistic regression model trained on New York Time's subscriber data and then test on Census demographic information to identify Which New Yorkers are likely to be subscribers and who is not.

The model should be deployed the next quarter to see if it helped add more New York subscribers than the previous quarter. 

### Acceptable Risks: 

- If the model classifies a likely subscriber as an unlikely subscriber 5% of the time. This can be mitigated by looking into why it is predicting wrong for this 5%, maybe there was a missing feature.
- If the model classifies an unlikey subscriber as a likely subscriber 5% of the time. 

### Alternative Solution: Use clustering to learn more about New York's subscriber group.

There are some ethical issues that can occur. If the model identifies likely subscribers based on high income and education, then there is a design bias. This can be mitigated by looking into features of readers who are interested in the content. There's the issue of consent, do subscribers know their data is being used to identify other likely subscribers?

Once New York Times has this model, they can decide on how and where to reach out to likely subscribers. Depending on budget, they could advertise through social medias or radio stations with messaging that entices their target groups.

## Data

The 5 year American Community Survey 2009 - 2019 was used to get precise demographic estimates of New York's demographics. I used age, gender, income, occuptation, education, ethnicity, and location data. After examining the distribution of each characteristic, I found some interesting insights.

- New York's labor force is made up of 50% of its population with the majority in civilian labor and less than one percent in the armed forces.						
- The education health, social services, administrative, science, retail, and financial services roles make up more than 52% of the workforce.						
- Non white races represent 40.6% of New York's population, making it more diverse than the USA's average of 23.7%.						
- New Yorkers 25 and older make up more than 97% of income earners.						

From there, I created three major adult age groups based on the Milennial, X, and Boomer generations. Noticeably, there are more Milennials with higher educations than the other groups. Gen X captures the highest shares of income over 75 thousand. The are 559,484 more females than males in the Boomer group. 

## Alogirthms

I used aggregate functions, vlookups, and pivot tables to clean and explore my data on excel. I created calculated fields in Tableau to represent income and education levels. 

## Tools

I used Python to scrape location data and call the Census Api. Excel to clean, manipulate, and perform analysis on the data. Tableau to visualize and map the data. 

## Communication

I will be pitching to the New York Time's marketing team.

## Links

- [Write up](https://github.com/Dong-Zhen/Relevance_of_NYT/edit/main/README.md)
- [Census Analysis on Google Sheets](https://docs.google.com/spreadsheets/d/1sxYRCKuNiGMVjmg1CprcZR_FmU6XC8IkZECXanqWy3o/edit?usp=sharing)
- [Tableau](https://github.com/Dong-Zhen/Relevance_of_NYT/tree/main/Tableau)
- [Powerpoint](https://github.com/Dong-Zhen/Relevance_of_NYT/blob/main/New%20York%20Times%20Opportunity.pdf)
