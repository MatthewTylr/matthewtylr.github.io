---
layout: post
title: Using Sentiment Analysis to Compare Inaugural Addresses for Obama and Trump
header-img: "img/trump_inauguration.jpg"
---

A month into Trump's presidency and it appears that he is going to be a divisive figure for the next four years. Regardless if you like him or not, I thought it would be interesting to perform some basic sentiment analysis on his inaugural address and compare it to someone else- say Barack Obama in 2009.

I thought this would be a somewhat apt comparison. Both Obama and Trump, while being opposite in the political spectrum, campaigned along similar lines. In 2008, Obama successfully pipped Hillary Clinton for the Democratic Nomination. Obama's background was certainly different than the pristine, well-manicured upbringings of other prominent politicians. This gave him more of a personality and zeal comparatively.

Flash forward to Donald Trump, and we have a somewhat similar story. Both candidates were unafraid to address major problems that seemed to be ailing the nation. For Obama, this was the War in Iraq and the economy. For Trump it was immigration and national security. Both candidates picked positive slogans and indicated some sort of positive reform and change in the government and direction of the country.

How were both of their campaign messages conveyed during their inaugural addresses? For this I snagged the text and took it to R. For the purpose of this post I looked mainly at net polarity for both sets of text. *Polarity is used to describe the positive and negative components of corpuses that make up a text.*

![ftd]({{ site.baseurl }}/img/inaug_sa_plot.png)
*Top: Bar graph showing total sum of corpus polarity. Bottom: Corpus polarity creep incremented by corpus ID.*

What is interesting is that they are both pretty positive speeches. In the future I would like to compile inaugural addresses of other prominent, and non-prominent, US presidents to observe the spectrum that it produces. Have there ever been overwhelmingly negative inaugural addresses?

#Sources:
[1] https://www.aol.com/article/news/2017/01/19/president-barack-obamas-first-inauguration-speech-full-text/21657532/
[2] http://www.cnn.com/2017/01/20/politics/trump-inaugural-address/
[3] https://www.r-bloggers.com/intro-to-text-analysis-with-r/

*Code available upon request!*