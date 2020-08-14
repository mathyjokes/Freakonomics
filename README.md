# What can you learn about on the Freakonomics Radio Podcast? 

An analysis of transcripts from 468 episodes over the past 10 years can tell you: people, time, and money.


The Freakonomics Radio Podcast hosts transcripts of their episodes on https://freakonomics.com/archive/. 
This project used Python (BeautifulSoup) to scrape these, and R (tidytext, udpipe) to extract keywords and phrases. 
Thanks very much to @amrwrites for their great article on using udpipe in R (https://towardsdatascience.com/easy-text-analysis-on-abc-news-headlines-b434e6e3b5b8), 
from which I pulled plenty of inspiration.

Freakonomics Radio invites listeners to "discover the hidden side of everything."
What keyword analysis shows is that Stephen Dubner and his guests talk about people and how they spend their time, above all else.
![noun_wordcloud](https://github.com/mathyjokes/Freakonomics/blob/master/freak_wordcloud_noun.png)

But it's not just what the podcast covers, but how it's saying it which can be interseting to prospective listeners.
A look at some of the most common adjectives used on the show display a pattern:
Dubner and his guests are discussing innovative ideas, described by adjectives such as "other," "good," "new," and "different."
![adj_barchart](https://github.com/mathyjokes/Freakonomics/blob/master/freak_common_adjs.png)

Looking beyond top phrases, we can consider phrases drawn out by Rapid Automatic Entity Extraction (RAKE).
Interestingly, many of these phrases appear to be guests' names. 
One non-name that stands out is "coronary artery," which is interesting because it is so unexpected - this is not a health podcast.
![rake](https://github.com/mathyjokes/Freakonomics/blob/master/freak_rake.png)
