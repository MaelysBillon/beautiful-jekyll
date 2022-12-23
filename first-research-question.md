---
layout: page
title: Who is the target audience?
subtitle: How does the public tolerate and appreciate violence in terms of tone and targets ?
---
* * *

Some visualiztion how violence is distributed among different genres 

<div class="flourish-embed flourish-survey" data-src="visualisation/12237943"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

Regression analysis to observe which type of violence contributes to a higher parental rating, i.e. is less tolerated, for the most popular genres in our dataset. 

<div class="flourish-embed flourish-chart" data-src="visualisation/12239226"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

TODO : ANALYZE THE PLOT



<div class="flourish-embed flourish-chart" data-src="visualisation/12251739"><script src="https://public.flourish.studio/resources/embed.js"></script></div>



### 1. Extraction of the parental advisory, explanation of the dataset

We can now analyze what is the tolerance per country about different types of violence. To do so, we have extracted the age advisory (parental certificate) from each country. Since there are missing values for countries, we decided to keep the certificates of few of them. We have in the following used dataset, film age advisories of 800 films and of 15 different countries : ['Argentina', 'Australia', 'Brazil', 'Canada', 'Finland', 'Germany', 'Ireland', 'Netherlands', 'Norway', 'Portugal', 'Singapore', 'South Korea', 'Spain', 'Sweden', 'United Kingdom'] from 1960 to 2010. To compare countries with each other we takes movies where certificates are available for each of these. We end up with a datset of 833 movies.

The following distribution represents film certifiactes available over the decades. 

<div class="flourish-embed flourish-chart" data-src="visualisation/12249745"><script src="https://public.flourish.studio/resources/embed.js"></script></div>


Here is a plot of the proportion of country producing films.

<div class="flourish-embed flourish-chart" data-src="visualisation/12248773"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

The extracted dataset contains a large majority of american films and were shot mostly in the 2000s.


The violence-type analysis is done using the data collected with the API and not using the summary. Information extracted from summaries are less precise since it do not reveal the content of the film, only it main synopsis. The API gives us the sensible content of the film incuding 'nudity', 'violence', 'profanity'. The following plot compares the type of violence extracted from the summaries versus the one extracted from the parental advisory.

Murders and wide-scale violence are more often detected by the summary extraction since it often appear to be a film topic present in the synopses while the explicit murder scenes do not appear. In the case of sexual abuse or torture, explicit violence may be present in certain scenes and may not appear in the summary of the film. 

<div class="flourish-embed flourish-chart" data-src="visualisation/12249292"><script src="https://public.flourish.studio/resources/embed.js"></script></div>


### 2. Analysis per country






