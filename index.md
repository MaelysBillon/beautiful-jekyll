---
layout: page
title: Representations of violence and public appraisal 
subtitle: Our data story
---
* * * 
# Representations of violence and public appraisal

## Abstract 
After the Aurora shooting in Colorado in July 2012 (twelve people killed and 58 others injured), during the premiere of The Dark Knight Rises, controversy arose around the release of the film Joker. Considered too violent, very strict security measures were taken before its theatrical release, where it is rated R. Violence has always been a pillar in media. From tragic Greek theater to public executions, its powerful emotional impact stirs attention. In films, violence can manifest in increased sensory details. The representation of violence can be, depending on the audience's appreciation, the era, the culture, more or less explicit, more or less tolerated with different stereotypes in play. Our project aims to analyze the co-dependency between public appraisal, tolerance, and representations of violence, under different dimensions such as financial success, the tone of the films (comedy or drama), and geo-political context (nation, era).

This data story studies the presence of violence in the [CMU Movie Summary Corpus](http://www.cs.cmu.edu/~ark/personas/). We use a bag-of-words approach to detect different types of violence in a movie summary. In particular, we lowercase the movie summary corpus and match only the base form of a word to include word variations. The following word cloud shows the 130 words in our violence dictionary colored by type of violence. A word's frequency in the movie summary corpus determines its size in the word cloud. 

<div class="flourish-embed" data-src="visualisation/12251430"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

TODO: appreciation / regression analysis of box office revenue / imdb rating 

After measuring the appreciation of violence, we want to evaluate the tolerance towards violence in movies. Furthermore, we want to determine if the context of violence influences tolerance. Our approach is to group the movies by genre and determine if the presence of a particular type of violence influences a movie's parental rating. Before doing that, we glimpse at the distribution of films through genres and determine popular types of violence in a genre. The following interactive graphic has one dot for each genre with more than 60 movies. A genre's popup shows the absolute number of films, the dominant type of violence, and each type of violence's percentage of films containing this kind of violence. The nodes can be sized by the forenamed ratios and absolute values and grouped by the dominant type of violence. Furthermore, one can filter for the ten most popular genres according to the number of movies. 

TODO: take into accout some results of the plot

<div class="flourish-embed flourish-survey" data-src="visualisation/12237943"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

Regression analysis to observe which type of violence contributes to a higher parental rating, i.e. is less tolerated, for the most popular genres in our dataset. 

<div class="flourish-embed flourish-chart" data-src="visualisation/12239226"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

TODO : ANALYZE THE PLOT

### 1. Extraction of the parental advisory, explanation of the dataset

We can now analyze what is the tolerance per country about different types of violence. To do so, we have extracted the age advisory (parental certificate) from each country. Since there are missing values for countries, we decided to keep the certificates of few of them. We have in the following used dataset, film age advisories of 800 films and of 15 different countries : ['Argentina', 'Australia', 'Brazil', 'Canada', 'Finland', 'Germany','Ireland', 'Netherlands', 'Norway', 'Portugal','Singapore', 'South Korea', 'Spain', 'Sweden', 'United Kingdom'] from 1960 to 2010. To compare countries with each other we takes movies where certificates are available for each of these. We end up with a datset of 833 movies.

The following distribution represents film certifiactes available over decades. 

<div class="flourish-embed flourish-chart" data-src="visualisation/12249745"><script src="https://public.flourish.studio/resources/embed.js"></script></div>


Here is a plot of the proportion of country producing films.

<div class="flourish-embed flourish-chart" data-src="visualisation/12248773"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

The extracted dataset contains a large majority of american films and were shot mostly in the 2000s.


The violence-type analysis is done using the data collected with the API and not using the summary. Information extracted from summaries are less precise since it do not reveal the content of the film, only it main synopsis. The API gives us the sensible content of the film incuding 'nudity', 'violence', 'profanity'. The following plot compares the type of violence extracted from the summaries versus the one extracted from the parental advisory.

Murders and wide-scale violence are more often detected by the summary extraction since it often appear to be a film topic present in the synopses while the explicit murder scenes do not appear. In the case of sexual abuse or torture, explicit violence may be present in certain scenes and may not appear in the summary of the film. 

<div class="flourish-embed flourish-chart" data-src="visualisation/12249292"><script src="https://public.flourish.studio/resources/embed.js"></script></div>


### 2. Analysis per country

