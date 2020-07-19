# Michelin Guide 2020
- Full analysis code - View <a href="https://nbviewer.jupyter.org/github/VajihaHameed/Portfolio/blob/master/Michelin-Guide-2020/Michelin%20star%20restaurants%202020.ipynb">here.</a>
- Web scraping/data gathering code - View <a href="https://nbviewer.jupyter.org/github/VajihaHameed/Portfolio/blob/master/Michelin-Guide-2020/Michelin%202020%20-%20Webscraping%20and%20data%20gathering.ipynb">here.</a>
- PDF of the below report, or continue to read below- View <a href=https://github.com/VajihaHameed/Portfolio/blob/master/Michelin-Guide-2020/Michelin%20Restaurants%20Analysis%20-%20Summary%20Report.pdf>here.</a>

## Contents

1. Executive Summary

2. Introduction
2.1 The Michelin Guide 2020
2.1.1 Awarding system
2.1.2 Timeline
	2.1.3 Criticisms

	2.2 The World’s 50 Best Restaurants
	2.2.1 Judging
	2.2.2 Timeline
	2.2.3 Criticisms

	2.3 Exploring both lists

3. Data

4. The Michelin Guide 2020
	4.1. Overview

	4.2. Cuisines

	4.3. United Kingdom

5. The Worlds 50 Best Restaurants
	5.1 Overview

	5.2 United Kingdom

6. Comparison of guides
	6.1 Michelin starred restaurants

7. Final Thoughts
	7.1 Further Analysis














## 1. Executive Summary

Amongst the culinary world, there are few greater accolades for a restaurant than being awarded a Michelin star (or three!), or being listed as one of the best in the world by reputable guides. Foodies and fine dine lovers, see the experience of dining at one of these award winning restaurants, as just that, an experience, and thus take to looking at guides such as The Michelin Guide and The World’s 50 Best Restaurants  - arguably the two most well known guides - to help determine which restaurant is next worth their time and money visit. 

But what is a Michelin star, what makes a restaurant worthy of being on this list and how is it awarded? How exactly does the spread of Michelin stars and the top 50 restaurants look like not only across the UK, but also the world, and what more can we understand about the types of restaurants that have received these awards? Ultimately, which list should a foodie be looking at?
By extensively scraping and compiling data to enable exploration of both The Michelin Guide and The World's 50 Best Restaurants list, we will set out in this analysis to find answers to the above and determine a pattern of the types of restaurants rated as the most worth visiting around the world - and come to a conclusion about which guide is the most influential, giving the most worthwhile information for those seeking the best culinary experiences.

The 2020 Michelin Guide, implemented across 31 countries worldwide at the time of writing, consists of 3,299 restaurants (this analysis will look at restaurants that have received one, two, or three Michelin stars, and does not contain other Michelin awards such as the Bib Gourmand). Japan leads with the most Michelin starred restaurants worldwide (669), and Japan, Italy and France make up half of the entire guide.
The World’s 50 Best Restaurants list 2019, includes restaurants from across 25 different countries, where Spain comes on top in the number of restaurants featured (7).

Of the 3,229 restaurants awarded Michelin stars:

2657 (81%) have been awarded one star
507 (15%) two stars 
35 (4%) three stars.

The UK sits 6th place in the hierarchy of countries with the most starred restaurants, with 169 starred restaurants spread country-wide across 83 cities/towns, broken down as:
144 one star restaurants
20 two star restaurants 
5 three star restaurants 
As can be expected, London has the lions share of these restaurants (63), however, outside of the capital, many of these restaurants are found in smaller towns or villages which one might not normally visit. Michelin describes 2 and 3 star restaurants as being of "excellent cooking that is worth a detour” or "exceptional cuisine that is worth a special journey”, which makes a rural getaway appealing to those seeking an exceptional dining experience. 2 restaurants from the UK have also made it onto the World’s 50 best restaurant list, both having 1 Michelin star and based in London.

Excitingly, for food lovers, the variety of cuisines included in The Michelin Guide is vast, with 103 cuisines included worldwide. However, modern cuisine takes the lead overall by a huge amount, accounting for 708 restaurants on the list (21%). In the UK, 65% of restaurants awarded with one or more Michelin star are classed as Modern Cuisine or Modern British, limiting the number of restaurants in the country to visit if one was looking for a more varied food offering. The second highest ranking cuisine for restaurants with Michelin stars is Japanese, however this is probably due to the number of restaurants in Japan awarded with stars, and most of the restaurants referring to their cuisine as “Japanese” even if they may also be classed as “Modern cuisine”. This does make us question how informative the cuisine category is on this list, when modern cuisine could mean a variety of things and have a number of overlaps with other cuisines.

We might assume that all the restaurants on the World 50 Best list would have at least one Michelin star, however in actual fact, included on the list, there are:
18 three Michelin star restaurants
9 two star
7 one star,
Leaving 16 restaurants with no star

We equally may think a country is more likely to be included in the top 50 list if it has more Michelin stars. However, delving into this further, we can see that is not necessarily the case. For instance:
Japan has the most restaurants featured in the Michelin Guide, however in the World 50 Best, Japan comes joint 4th with 5 other countries, with the percentages differing greatly between both guides (20.3% vs 4.1%).
Spain, which has the most restaurants in the top 50 (7 restaurants accounting for 14% of all the restaurants on the World 50 best list), has a 6.5% share of restaurants in The Michelin Guide.

The Michelin Guide does not yet cover all of the world, which can account for some of the disparity in these lists. There are 16 countries which feature both in The Michelin Guide and The World’s 50 Best, and 8 countries which aren’t yet included in the scope of The Michelin Guide. 
However 4 of the top 50 restaurants (8%) are in countries where the guide exists, which does make us wonder why they weren’t deemed “good enough” to be awarded a Michelin star, but were chosen by the Word 50 Best panel, to be amongst the best restaurants in the world.
This brings into question the judging criteria for both guides. Some have argued that The World 50 Best Restaurants list, emphasises restaurants involved in molecular gastronomy more over other types of restaurants -which may mean judges are more naturally biased towards these types of establishments.

It does however appear that for the most part, the two guides complement each other, rather than contradict. With 76% of restaurants listed in the World 50 Best list also having been awarded one Michelin star or more, it does seem as though judges from both guides are having the same exceptional dining experiences at these establishments. 

For now, foodies and those looking for gastronomic experiences, will probably continue to look at both these guides side by side to plan which restaurant will be next on their bucket list. Countries and restaurants featured on both lists, in particular the three Michelin starred, are certainly deemed high on the culinary destination list, many of which will have booked out waiting lists from eager diners. Certainly, heading to a country that excels in both of the lists (such as Japan or France) , would be a destination for a “foodie expedition”,







## 2. Introduction

Amongst the culinary world, there are few greater accolades for a restaurant than being awarded a Michelin star (or three!), or being listed as one of the best in the world by reputable guides. Foodies and fine dine lovers, see the experience of dining at one of these award winning restaurants, as just that, an experience, and thus take to looking at guides such as The Michelin Guide and The World’s 50 Best Restaurants  - arguably the two most well known guides - to help determine which restaurant is next worth their time and money visit.

### 2.1 The Michelin Guide 2020

The Michelin Guide is an annual guide published by the tyre company Michelin, listing the very best in dining experiences across the world, through a star rated awards system. It is arguably the most well known and revered guide of its kind in the world. The very first Michelin Guide was compiled in 1900 by the Michelin brothers, however the star awarding system started in 1926 in France, with the first stars awarded in the UK in 1974. New York was added to the guide in 2006 and it crossed over to Asia in 2007.

The guide states the following definitions for each of the Michelin star awards:

One star: "a very good restaurant"
Two stars: "excellent cooking that is worth a detour”
Three stars: "exceptional cuisine that is worth a special journey”

2.1.1 Awarding system
There are approximately 120 Michelin inspectors worldwide, who spend 3 weeks out of 4 on the road in a particular region, travelling to a different restaurant every day if possible for both lunch and dinner. The exact process of how a Michelin star is awarded to a restaurant has been a very closely guarded secret, however some details have come to light over the years. What is known is that inspectors will visit a restaurant multiple times in a year, when it is being considered for an additional star (or its first star), or if a star might be taken away. 

Restaurants are supposedly awarded stars based on the following criteria, however the exact nature is unknown: “quality of the ingredients used, mastery of flavour and cooking techniques, the personality of the chef in his cuisine, value for money and consistency between visits.”

2.1.2 Timeline

Each country’s guide is announced at different times of the year. In the UK, the list is announced in October of the year before. ie. the 2020 list which is explored later, was announced in October 2019.

2.1.3 Criticisms

The guide has been criticised for giving unfair bias towards French restaurants - both French cuisine worldwide, and restaurants in France itself.

There have been similar criticisms about the guide being too lenient with restaurants in Japan, given the large number of awards given in the country. However this allegation was counteracted by the fact that there are far greater restaurants in the larger Japanese cities comparatively to other large cities across the world. Eg. Paris has approx 40,000 restaurants, whereas Tokyo has around 160,000 restaurants.

### 2.2 The World’s 50 Best Restaurants 2019

The World’s 50 Best Restaurants Guide is an annual ranking of restaurants across the world, deemed to be the best in the world by a panel of chefs, food writers and culinary experts. It first appeared in the magazine Restaurant in 2002 and since has grown to become one of the main influencers in the restaurant industry, worldwide.

This list is often cited in publications around the world, including The Telegraph and as such, has now become one of the leading guides on gastronomy around the world. As with The Michelin Guide, restaurants that find themselves in this list, have a surge of reservations and flocks of diners wanting to visit, so it is an accolade that is highly sought after by chefs.

2.2.1 Judging

Taken from its website: “The World's 50 Best Restaurants list is compiled from the votes of the "World’s 50 Best Restaurants Academy", a group of 26 panels established to make the ranking. The world is divided into regions, with a chairperson in each region appointed for their knowledge of their part of the restaurant world. These chairs each selected a voting panel of 40 members, who every year cast thousands of votes.
There is no list of nominees; each member of the international voting panel votes for their own personal choice of ten restaurants. Up to six votes can be cast for restaurants in the voter's own region, while at least four must go to restaurants outside of the home region. No voting member is allowed to vote for their own restaurant, or one in which they have an economic interest, and voters must have eaten in the restaurants they nominate within the past 18 months. The integrity of the voting process and the resulting list is adjudicated by global consultancy firm Deloitte.” 

More information about the voting process can be found here.

2.2.2 Timeline

The new list is announced in June each year, ie. the 2019 list was announced in June 2019.

2.2.3 Criticisms

The list has been criticised in the past for being very euro-centric, with the majority of restaurants included in the list based in Europe. There have also been accusations of sexism within the list, with a limited representation of female chefs.

In 2019, the organisers also decided controversially, to disqualify restaurants that had previously taken the number one spot in a previous list from the subsequent lists - moving them to “The Best of the Best” category. This has been a cause of uproar amongst top chefs, and has meant the list has lost some of its credibility as it no longer includes “all” of the best restaurants whilst excluding some. 

There have been rumours of rigged ranking, due to the system in which the panel can vote for their personal choice, however the guide refutes this, explaining that the process is adjudicated and fair. 

2.3 Exploring both lists
So how exactly does the spread of Michelin stars and the top 50 restaurants look like not only across the UK, but also the world? Are the same restaurants included in both, as one might expect - and what more can we understand about the types of restaurants that have received these awards? 

As both guides are held so highly in the culinary world, we think that the results of both should run somewhat parallel to each other. By exploring both The Michelin Guide and The World's 50 Best Restaurants list, can we determine if there is in actual fact a correlation with restaurants included in the list and those given Michelin stars?


## 3. Data

Data for this project was compiled through extensive web scraping of the current editions of each of the online Michelin Guides for every country currently partaking in the awards, and The World’s 50 Best Restaurant 2019 online list. The full Jupyter script for this web-scraping is <a href="https://nbviewer.jupyter.org/github/VajihaHameed/Portfolio/blob/master/Michelin-Guide-2020/Michelin%202020%20-%20Webscraping%20and%20data%20gathering.ipynb">here.</a>. 

This data was then used to do a thorough analysis, the main findings of which are contained in this report. The full data analysis script can be found <a href="https://nbviewer.jupyter.org/github/VajihaHameed/Portfolio/blob/master/Michelin-Guide-2020/Michelin%20star%20restaurants%202020.ipynb">here.</a>. The links to every interactive visualisation in this report, are found below or above each plot, and to view all interactive charts online, click [here](https://chart-studio.plotly.com/~Jia24/).

Tools and libraries used for this analysis, all in Python: Jupyter notebook, BeautifulSoup, Pandas, NumPy, Seaborn, Plotly.


## 4. The Michelin Guide 2020

### 4.1 Overview

There are 3,299 restaurants included in The Michelin Guide worldwide, compiled of individual guides from 31 countries. The following countries are included in the guide at the time of writing (Feb 2020):

Austria, Belgium, Brazil, China, Croatia, Czech Republic, Denmark, Finland, France, Germany, Greece, Hong Kong, Hungary, Ireland, Italy,  Japan, Luxembourg, Macau, Netherlands, Norway, Poland, Portugal, Singapore, Spain, South Korea, Sweden, Switzerland, Taipei, Thailand, UK, United States.

Of these 31 countries, the ten with the most starred restaurants (note that at this point, we are looking at the number of restaurants, not the total number of stars) are: 

![Fig20](https://github.com/VajihaHameed/Portfolio/blob/master/Michelin-Guide-2020/Images/fig20.png)

Japan leads with the most stars worldwide, with UK coming in 6th place. We can further analyse this breakdown of stars per country, looking at how many 1 star, 2 star and 3 star restaurants there currently are in each country in the chart below. 
View the interactive plot [here.](https://chart-studio.plotly.com/~Jia24/6/#/) 

![Fig1](https://github.com/VajihaHameed/Portfolio/blob/master/Michelin-Guide-2020/Images/fig1.png)

We can also visualise this information on a world heat map. Find the interactive version of this [here.](https://chart-studio.plotly.com/~Jia24/8.embed)
![Fig2](https://github.com/VajihaHameed/Portfolio/blob/master/Michelin-Guide-2020/Images/fig2.png)

Looking at the proportional breakdown of restaurants across the world included in the guide, we can see that Japan, France and Italy make up 50% of the entire list. Interactive chart [here.](https://chart-studio.plotly.com/~Jia24/10.embed)

![Fig12](https://github.com/VajihaHameed/Portfolio/blob/master/Michelin-Guide-2020/Images/fig12.png)

There are 2657 (81%) one star restaurants, 507 (15%) two star and 135 (4%) three star included in the guides worldwide. It indeed does seem that gaining three stars is a very rare achievement amongst restaurants. Japan has the most 3 star restaurants, followed by France, Italy and Germany, which follows the pattern of countries with the most starred restaurants.
![Fig14](https://github.com/VajihaHameed/Portfolio/blob/master/Michelin-Guide-2020/Images/fig14.png)

### 4.2 Cuisines

There are 103 different cuisines included in the data. It is worth noting that there are some overlaps in a handful of cuisine names, for instance 'French' and 'Classic French’, 'Creative British' and 'Modern British'. However further investigation into this showed that this does not skew the analysis in a way which requires any further manipulation of this data.

We will explore these cuisines in two different ways:
The number of restaurants of a certain cuisine, which have one star or more
The total number of stars for each cuisine. ie. if a restaurant has 3 stars, all three will be added to the total of stars in this cuisine


The top 10 cuisines with the most starred restaurants are:

![Fig18](https://github.com/VajihaHameed/Portfolio/blob/master/Michelin-Guide-2020/Images/fig18.png)

The cuisine with the most restaurants included in the guide is Modern Cuisine.

The top 10 cuisines with the most stars overall are:

![Fig19](https://github.com/VajihaHameed/Portfolio/blob/master/Michelin-Guide-2020/Images/fig19.png)

The cuisine with the most stars is also modern cuisine, and the majority of this top 10 list is the same as the top cuisines with the most restaurants.

We can visualise both of these breakdowns of cuisine in a scatter plot. Click [here](https://chart-studio.plotly.com/~Jia24/12.embed) to view the interactive zoomable version. 

![Fig3](https://github.com/VajihaHameed/Portfolio/blob/master/Michelin-Guide-2020/Images/fig3.png)

We can see there is a difference between the two sets of data in particular for Creative, Japanese contemporary and Modern cuisine, from which we deduce that these cuisines most likely have more restaurants with the higher number of stars. The table below delves into this further, looking at which cuisines have 3 star restaurants. 

Upon further investigation, 20 cuisines out of the 103 have three star restaurants (19%). From the table below, we can see that the Creative, Japanese and Modern cuisines do indeed have the highest number of restaurants with the highest 3 star accolade.

![Fig17](https://github.com/VajihaHameed/Portfolio/blob/master/Michelin-Guide-2020/Images/fig17.png)

The chart below visualises this information. View interactive version [here](https://chart-studio.plotly.com/~Jia24/14.embed).

![Fig4](https://github.com/VajihaHameed/Portfolio/blob/master/Michelin-Guide-2020/Images/fig4.png)

The heat map shows further the correlation between cuisines and number of stars.

![Fig5](https://github.com/VajihaHameed/Portfolio/blob/master/Michelin-Guide-2020/Images/fig5.png)


The second highest ranking cuisine for restaurants with Michelin stars is Japanese, however this is probably due to the number of restaurants in Japan awarded with stars, and most of the restaurants referring to their cuisine as “Japanese” even if they may also be classed as “Modern cuisine”. This does make us question how informative the cuisine category is on this list, when modern cuisine could mean a variety of things and have a number of overlaps with other cuisines.

Taking a further look at this, Japan’s breakdown of cuisines is: 296 Japanese, 121 French, with the remaining restaurants were majority all derivates of Japanese cuisine( such as Ramen, Sushi, Soba), proving our assumption, approx 80% of Michelin starred restaurants in Japan are of (or a derivate of) Japanese cuisine.

### 4.3 United Kingdom

In the United Kingdom, there are 144 one star restaurants, 20 two star restaurants and 5 three star restaurants. The majority of Michelin rated restaurants in the UK have 1 star, with a small percentage having 2 or 3 stars.
![Fig6](https://github.com/VajihaHameed/Portfolio/blob/master/Michelin-Guide-2020/Images/fig6.png)
![Fig7](https://github.com/VajihaHameed/Portfolio/blob/master/Michelin-Guide-2020/Images/fig7.png)
Michelin starred restaurants in the UK are spread across 83 different cities, the top 10 of which can be seen below. (The areas shown with 2 restaurants are listed in alphabetical order, there are more locations in the UK which are joint in this 6th place ranking that aren’t shown in this snapshot of 10):

![Fig22](https://github.com/VajihaHameed/Portfolio/blob/master/Michelin-Guide-2020/Images/fig22.png)

London by far has the most starred restaurants, with Birmingham second, which is expected, What is interesting is that the bigger the city does not mean the more starred restaurants. As we would expect Manchester, Leeds and Sheffield to be the next in this list if we going by this rule. However Sheffield is not included in the list at all. Many of these restaurants outside of London are in actual fact in more rural villages or towns, rather than cities.

Viewing this on a graph shows us where this lions-share sits. See the interactive chart [here](https://chart-studio.plotly.com/~Jia24/16.embed). 

![Fig8](https://github.com/VajihaHameed/Portfolio/blob/master/Michelin-Guide-2020/Images/fig8.png)

By also visualising this spread on a bubble map of the UK, the can see the restaurants are indeed spread across the entirety of the UK, but there are significantly more in the South than in the North.

View the interactive map [here](https://chart-studio.plotly.com/~Jia24/18.embed). 
![Fig9](https://github.com/VajihaHameed/Portfolio/blob/master/Michelin-Guide-2020/Images/fig9.png)

Upon exploring the cuisine breakdown of UK restaurants in the guide, the majority of restaurants are Modern Cuisine (53) or Modern British (41), both of which combined account for 65% of the 144 UK restaurants in the guide. View the interactive chart [here](https://chart-studio.plotly.com/~Jia24/31.embed).
![Fig23](https://github.com/VajihaHameed/Portfolio/blob/master/Michelin-Guide-2020/Images/fig23.png)


## 5. World’s best 50 restaurants 2019

Now we will investigate further the data scraped from The World's 50 Best Restaurants 2019 list.

N.B. This list usually comes out in June each year for the current year. Whereas the Michelin list in the UK comes out in October of the previous year - ie. the 2020 list was announced in October 2019. For this reason, at the time of writing this report (Feb 2020), the 2020 Michelin guide's equivalent world’s best 50 restaurant list is from 2019.

### 5.1 Overview

The restaurants in the 2019 top 50 list are spread across 25 countries. The 5 countries with the most restaurants listed in the guide are:

![Fig21](https://github.com/VajihaHameed/Portfolio/blob/master/Michelin-Guide-2020/Images/fig21.png)

All 25 countries in the list are visualised in the chart below.
![Fig10](https://github.com/VajihaHameed/Portfolio/blob/master/Michelin-Guide-2020/Images/fig10.png)

We can also visualise this on world heat map. View interactive map [here](https://chart-studio.plotly.com/~Jia24/23.embed).
![Fig11](https://github.com/VajihaHameed/Portfolio/blob/master/Michelin-Guide-2020/Images/fig11.png)


There are 18 three star restaurants, 9 two star, and 7 one star restaurants on the list. View interactive plot [here](https://chart-studio.plotly.com/~Jia24/27.embed).
![Fig15](https://github.com/VajihaHameed/Portfolio/blob/master/Michelin-Guide-2020/Images/fig15.png)

### 5.2 United Kingdom

The UK comes in joint 4th place on the list, with 6 other countries. Having 2 UK based restaurants in The World’s 50 Best list, The Clove Club and Lyle’s, the UK has 4% of the best restaurants in the world according to this guide. 

The two restaurants are based in London - with approximately 15,500 restaurants in London, compared to 26,000 in the entire UK, this comes as no surprise.
It is interesting that both of these restaurants are in Shoreditch, the same borough of London, have 1 Michelin star each and both are of Modern Cuisine.


## 6. Comparison of both guides

We will now look at how the two guides either complement or contradict each other and what we can deduce from looking at them together.

We would assume, that if a country had more restaurants with stars, that the country is more likely to be on The World’s 50 Best Restaurant list - and vice versa. However, delving into this further, we can see that is not necessarily the case.

Spain, which has the most restaurants in the top 50 (7 restaurants), accounting for 14% of all the restaurants on the list has a 6.46% share of The Michelin Guide. 
On the other hand, we know there are 2 UK based restaurants on the world 50 best list, equating to 4%, comparative to 5.12% in the Michelin Guide, which is more of a comparative proportion.

Of the 25 countries that have made it onto The World’s 50 Best list, there are 17 countries which feature in The Michelin Guide also. 
We can see from the chart below that for some of these countries, their presence in both guides differs greatly. For instance, Japan has the most restaurants featured in The Michelin Guide, however in The World 50 Best, Japan comes joint 4th with 5 other countries, with the percentages extremely different (20.3% vs 4.1%). View interactive plot [here](https://chart-studio.plotly.com/~Jia24/25.embed).

![Fig13](https://github.com/VajihaHameed/Portfolio/blob/master/Michelin-Guide-2020/Images/fig13.png)
Why might that be? One of the main reasons may well be that The Michelin Guide does not yet cover the entire world, whereas The World 50 Best, according to it’s website and its name. does indeed cover the world - or more of it, so there may be less scope for example, Japanese restaurants, to take a bigger chunk of the top 50. Another reason, could be that The World 50 Best may have a more Eurocentric approach, as it has been criticised to have so in the past, so it may be more bias towards neglecting the Asian countries. The organisers do however claim that their process is fair and unbiased.

The remaining 8 countries included The World 50 Best, where The Michelin Guide does not yet stretch, account for 11 restaurants on the list. Those countries are:

Peru
Mexico
Russia
Chile
Argentina
Slovenia
South Africa
Colombia


### 6.1 Michelin starred restaurants

As outlined in the introduction, three stars are defined by the Michelin Guide as a restaurant worthy of a special trip - the best of the best. We therefore might have assumed that all the restaurants named as the 50 best in the world, would be of three Michelin star calibre (excluding the 11 restaurants on this list we determined earlier ,that reside in countries where The Michelin Guide exists).

However, this isn’t the case, as the below chart shows. 34 of The World's 50 Best Restaurants have one or more Michelin stars (18 three star restaurants, 9 two star, and 7 one star restaurant), leaving 16 restaurants classed as being the “best in the world” which do not have the award of one Michelin star or more. The chart below takes a closer look at the breakdown of Michelin starred restaurants in The World 50 Best list. View interactive plot [here](https://chart-studio.plotly.com/~Jia24/29.embed).

![Fig16](https://github.com/VajihaHameed/Portfolio/blob/master/Michelin-Guide-2020/Images/fig16.png)
Whilst not all are of three Michelin star quality, it does follow our instinct however that proportionally, to how many three star restaurants there are worldwide, the proportion on this top 50 list (36% three star, 18% two star, 14% one star, 32% no star) is higher than in The Michelin Guide itself ()- hence reinforcing the three Michelin star accolade as a mark of a truly special restaurant.

Five of the countries included in The Michelin Guide, have a restaurant listed in the World’s 50 Best, that do not have a Michelin star. These countries are:

Brazil
Thailand
United States
Germany
China

However, Gaggan, in Thailand, closed down shortly after the World 50 Best Restaurant list was announced in 2019, so in actual fact,  there are 4 restaurants/countries on this list.

This means that 8% of restaurants on the World 50 Best list, were not deemed 'special enough' by The Michelin Guide to be awarded a star - but were deemed by the Word 50 Best panel, to be amongst the best restaurants in the world. This brings into question the judging criteria for both guides. Some have argued that The World 50 Best Restaurants list, emphasises restaurants involved in molecular gastronomy mores over other types of restaurants - whereas The Michelin Guide is perhaps more inclusive. 

We can therefore conclude, that out of the 50 on The World’s 50 Best, 8 restaurants are in countries where there is no Michelin Guide and 4 are in countries where there are Michelin Guides, but have not been awarded stars. Other than those restaurants, the remaining (76%), all belong on both lists, revering them amongst the culinary world as truly being fantastic restaurants deemed a visit.


## 7. Final thoughts

The Michelin Guide was established more than a century ago, making it the most well established  guide in circulation, and arguably the most reputable and sought after, for this very reason. However, it’s secrecy and lack of transparency in the process behind how stars are awarded, has been a cause for criticism by some, who have questioned the impartiality of the awards.

On the other hand, The World’s 50 Best clearly lays out the process by which it is compiled, with an emphasis on trying to show how it is both fair and regulated (although this has been questioned too). The ranking is decided by a group of over a thousand chefs, critics and experts, most of which are well known and highly respected in their field - unlike the Michelin Guide, where around 120 anonymous inspectors are the judges.
One could argue that for a chef, they would receive more gratification by being listed as one the world’s best 50 by their peers, whereas the general public may be more inclined to trust the judging of the anonymous “civilian” inspectors.

Modern cuisine and Japanese cuisine play a significant part in restaurants awarded stars, however, the cuisine category is questionable, as there may be many overlaps within these cuisines eg. French cuisine could also be modern.

It does appear that for the most part, the two guides complement each other, rather than contradict. With 76% of restaurants listed in the World 50 Best list also having been awarded one Michelin star or more, it does seem as though judges from both guides are having the same exceptional dining experiences at these establishments. 

For now, foodies and those looking for gastronomic experiences, will probably continue to look at both these guides side by side to plan which restaurant will be next on their bucket list. Countries and restaurants featured on both lists are certainly deemed high on the culinary destination list, many of which will have booked out waiting lists from eager diners.

### 7.1 Further analysis

As the Michelin Guide evolves into new territories and opens up its doors to more of the world, it will be interesting to see how this comparison changes, and if the two lists become even more alike.

It will be worthwhile to delve into deeper analysis to further our understanding of the fine dining world. Comparing previous years’ Michelin Guides and World 50 Best, with the 2019/20 lists will broaden this analysis. Looking closer at other well known guides such as The Good Food Guide will also expand our knowledge of this culinary world and perhaps bring up more “food for thought”.


