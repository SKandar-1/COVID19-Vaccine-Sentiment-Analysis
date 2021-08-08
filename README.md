__Title:__ COVID19 Vaccine Sentiment Analysis

__Abstract:__ 

As the delta variant of COVID19 spreads rapidly throughout the world, countries are in a race to vaccinate people sooner than the virus can spread. While in some countries the vaccines are in short supply, in other countries some people are reluctant to take the vaccine for various reasons. To understand public sentiment about COVID19 vaccines, it is worthwhile to study tweets for sentiment analysis since twitter is one of the prominent social media platforms where people share their opinions. In this study, tweets about COVID19 vaccines showed 37% neutral, 47% positive, and 16% negative sentiments. Word Cloud of the positive tweets show the words ‘safe’, ‘effective’, ‘good’ whereas that of the negative tweets show the words ‘side effect’, ‘risk’, ‘concern’, ‘scary’, etc.. Presumably, people with positive sentiment are more optimistic about the benefit of the vaccine whereas people with negative sentiments are concerned about side effects of the vaccine.

__Introduction:__

Delta variant (B.1.617.2. variant) is a SARS-CoV-2 mutation that originally surfaced in India in December 2020 and then rapidly spread in the other parts of the world including Great Britain and the US.(Reference 1) WHO described this variant as ‘more contagious and fittest’ and CDC described this variant as ‘variant of concern’ and particularly dangerous towards unvaccinated people. At present, the delta variant accounts for 82% of COVID cases in the US.(Reference 2) Although scientific studies have shown the COVID19 vaccines are effective towards the delta variant, people are hesitant to take the vaccine for vaions reasons; social, religious, political, etc.(Reference 3) In this study, I analyzed public sentiments about COVID vaccines in related tweets and tried to identify key words related to positive and negative sentiments by data visualization in Word Cloud. 

__Methodology:__

1. Tweets about COVID19 were obtained by querying ‘#COVID19vaccines’ in Twitter’s API using tweepy library. 
2. All tweets were saved in a variable using python list-comprehension and a pandas DataFrame was created from the variable.
3. DataFrame was cleaned for any hyperlinks and any strings with  #.
4. Subjectivity, polarity, followed by sentiments of the tweets were obtained using TextBlob library.
5. DataFrame was checked for any duplicates and missing values.
6. Subjectivity and polarity was plotted in a scatter plot (Figure 1) using matplotlib and pyplot libraries.
7. Neutral, positive, and negative sentiment tweet counts were plotted in a bar plot (Figure 2).
8. Word Clouds were generated for both positive and negative sentiment tweets after removing stop words from both categories (Figure 3,4).(Reference 4)

![](https://github.com/SKandar-1/Figures/blob/main/COVID%20Sentiment%20Analysis%20Scalletr%20Plot.png)

__Figure 1:__ COVID Vaccine Sentiment Analysis Scatter Plot

![](https://github.com/SKandar-1/Figures/blob/main/COVID%20Sentiment%20Analysis%20Bar%20Plot.png)

__Figure 2:__ COVID Vaccine Sentiment Analysis Bar Plot

![](https://github.com/SKandar-1/Figures/blob/main/COVID_Vaccine_Pos_entiment_WordCloud.png)

__Figure 3:__ WordCloud for COVID Vaccine Positive Sentiment Tweets

![](https://github.com/SKandar-1/Figures/blob/main/COVID_Vaccine_Neg_entiment_WordCloud.png)

__Figure 4:__ WordCloud for COVID Vaccine Negative Sentiment Tweets

__Results:__

In this study tweets about COVID19 vaccines showed 37% neutral, 47% positive, and 16% negative sentiments. Word Cloud of the positive tweets show the words ‘safe’, ‘effective’, ‘good’, ‘protect’ whereas that of the negative tweets show the words ‘side effect’, ‘risk’, ‘concern’, ‘GOP’,. Presumably, people with positive sentiment are more optimistic about the benefit of the vaccine whereas people with negative sentiments are concerned about side effects of the vaccine and some political reasons.

__Conclusions:__

Although Twitter flags and even removes misinformation about COVID19 vaccines from the platform, there are still some negative sentiments and hesitency about the vaccine’s efficacy, negative side effects, etc. More scientific experiments on the vaccine’s effectiveness, side effects and education will probably help more populations get vaccinated and slow/stop the spreading of the highly contagious delta variant of COVID19.

__References:__

1. https://www.yalemedicine.org/news/5-things-to-know-delta-variant-covid
2. https://covid.cdc.gov/covid-data-tracker/#variant-proportions
3. https://health.ucdavis.edu/coronavirus/covid-19-information/delta-variant.html
4. https://www.youtube.com/watch?v=ujId4ipkBio&t=226s

