# Covid19-Traffic-Data-Analysis

Full Report: https://docs.google.com/document/d/1vWSOlanaCzHeue3ymjtmIb--68ndoZCDMxYTpWqoTGw/edit#

Problem:
Pre-lockdown, telework was not nearly as popular as it is now. Many employers have started offering remote work/flexible work options (PwC, for example, announced that all employees are eligible for fully remote work). In our EDA, we noticed that there was a clear decrease in travel times post-lockdown, as well as a spike in average speeds. As such, it seems that the share of the population teleworking does affect travel times. 
This shift to permanent remote work is unprecedented, and could have major effects on future traffic and thus, city planning. As such, our model seeks to predict travel times based on how much of the population is teleworking, to help better understand what our future’s traffic could look like. To predict how prevalent teleworking became across different tracts, multiple factors of the tract need to be taken into consideration.

Hypothesis:
In constructing our model, we hypothesize that travel times are negatively correlated with median income per tract.
Geographic, demographic, and socioeconomic factors of a tract can serve as reasonable features for a multiple regression model to predict post-lockdown travel times.
We are using average income as a proxy for how much of the population is teleworking, because that data is not possible to find at the granularity that we want. However, according to the Census Bureau’s Household Pulse Survey, the higher earning households switched to telework during the pandemic (for example, households >$200k, 73.1% switched) more than lower earning households (<$25k, only 12.7% switched). Based on that, tracts with higher average incomes are more likely to have a larger share of the population switch to telework, resulting in decreased traffic, faster average speeds, and overall, lower travel times. Thus, as a starting point, we will base a linear model on the median income to predict travel times.

