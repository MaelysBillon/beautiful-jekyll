---
layout: page
title: Tolerance and Appreciation of Violence
subtitle: How successful are violent movies? In which genres is violence more tolerated?
---
* * *

This data story studies the presence of violence in the [CMU Movie Summary Corpus](http://www.cs.cmu.edu/~ark/personas/). We use a bag-of-words approach to detect different types of violence in a movie summary. In particular, we lowercase the movie summary corpus and match only the base form of a word to include word variations. The following word cloud shows the 130 words in our violence dictionary colored by type of violence. A word's frequency in the movie summary corpus determines its size in the word cloud. 

<div class="flourish-embed" data-src="visualisation/12251430"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

TODO: appreciation / regression analysis of box office revenue / imdb rating 

After measuring the appreciation of violence, we want to evaluate the tolerance towards violence in movies. Furthermore, we want to determine if the context of violence influences tolerance. Our approach is to use the genre of a movie as a proxy for the context of violence. First, we catch a glimpse of the distribution of films through genres and determine popular types of violence in a genre. The following interactive graphic has one dot for each genre with more than 60 movies. A genre's popup shows the absolute number of films, the dominant type of violence, and each type of violence's percentage of films containing this kind of violence. The nodes can be sized by the forenamed ratios and absolute values and grouped by the dominant type of violence. Furthermore, one can filter for the ten most popular genres according to the number of movies. 

<div class="flourish-embed flourish-survey" data-src="visualisation/12237943"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

We observe that murder and wide-scale violence are the dominant types of violence. Furthermore, the presence of any violence, murder, wide-scale violence, and other violence is about of the same order of magnitude across all genres. However, some genres are prone to torture and sexual violence, but others are not. For example, a third of all movies in adult genres contain sexual violence, whereas less than 5% of all comedies have sexual violence. For torture, we can draw a similar picture - it is more common among slasher (46%), cult (33%), and horror (31%) movies and less common for romance (6.9%) and comedy (8.4%) movies. 

Now we dive deeper into violence in genres and analyze for the ten genres with the most movies how the presence of a type of violence contributes to a parental rating of a film. We use the [parental rating certificates](https://help.imdb.com/article/contribution/titles/certificates/GU757M8ZJ9ZPXB39?ref_=helpart_nav_27#) that we scraped from [IMDB](https://www.imdb.com). We average all available parental ratings of different countries for each film. Averaging gives us one minimum age per film that certificate authorities recommend for people to watch this movie. Afterward, we do a regression analysis with the mean parental rating as the outcome and the type of violence indicators as binary predictors. The plot below shows the regression coefficients. The intercept denotes the average parental rating for a movie with no detected type of violence. 

<div class="flourish-embed flourish-chart" data-src="visualisation/12239226"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

Overall genres, the presence of other violence has a not significant or small significant positive or negative contribution to the parental ratings. Interestingly, the existence of wide-scale violence tends to reduce the parental rating. The presence of torture, sexual violence, or murder increases a film's parental rating by more than two years on average. The tolerance towards murder and torture is volatile across genres. Consider horror movies and thrillers. Both have a high parental rating without the presence of any violence. However, thrillers tolerate murder more than horror movies, but horror movies tolerate torture more than thrillers. The tolerance towards sexual violence is more constant. Its presence adds at least 1.1 years to the parental rating in any of the most popular genres.  Fascinating are also comedies. Without any violence, they have a lower parental rating than the average movie without violence. However, they are more tolerant of torture and murder. 






