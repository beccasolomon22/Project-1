# TikTok Usage and COVID-19
Team 3 Members: Mustafa Naeem, Rebecca Solomon, Francis Crawford, Isabelle Roetcisoender, & Sabrina Fernandez

## Topic Overview
In the wake of the coronavirus (COVID-19) pandemic many have been turning to social media for information, support and social connection. This analysis serves to answer how social media usage has been impacted by the coronavirus (COVID-19) pandemic. 

* How has TikTok screentime increased since the pandemic?
* How has revenue and the number of subscribers increased since the pandemic?
* How has social media screentime increased since the pandemic? 


## Datasets

[Children's Screentime](https://www.webmd.com/parenting/news/20221114/kids-screen-time-rose-sharply-during-pandemic-study-says#:~:text=The%20increase%20amounts%20to%20an,study%20published%20in%20JAMA%20Pediatrics)

[US vs Global Screentime](https://www.comparitech.com/tv-streaming/screen-time-statistics/#:~:text=Worldwide%2C%20the%20average%20person%20spends,minutes%20of%20listening%20to%20podcasts)

[Changes and correlates of screen time in adults and children](https://www.thelancet.com/action/showPdf?pii=S2589-5370%2822%2900182-1)

[Social Media Stock](https://www.kaggle.com/datasets/prasertk/major-social-media-stock-prices-20122022)

[Company by Age]()

[TikTok Revenue and Users]()

[Total Revenue for Different Social Media Sites](https://www.kaggle.com/datasets/prasertk/major-social-media-stock-prices-20122022?resource=download)

[Revenue for Streaming Sites](https://www.kaggle.com/code/lamaradwan/netflix-and-tiktok-revenue-and-users/input)

[TikTok Reviews 2015-2021](https://www.kaggle.com/datasets/shivamb/35-million-tiktok-mobile-app-reviews)

[TikTok Reviews 2022](https://www.kaggle.com/datasets/shivkumarganesh/tiktok-google-play-store-review)


## Data Cleaning/Manipulation & Conversion

![IMG1](https://github.com/isabelleroet/tiktok/blob/f6b0056728c649d71ff33d8df1849d8cc870399c/tiktokimg/Screenshot%202023-03-27%20at%201.04.58%20AM.png)
For getting the company ages, we did the same thing, but we also set the csv columns as variables and plotted a bar graph using pandas as well.

![IMG2](https://github.com/isabelleroet/tiktok/blob/f6b0056728c649d71ff33d8df1849d8cc870399c/tiktokimg/Screenshot%202023-03-27%20at%201.03.46%20AM.png) For getting the average screen time graphs, we passed the 2 csvs through the reader: 1 for average screen time in 2018 and 1 for average screen time in 2023; the information for average screen time from 2020 to 2022 was retrieved from the WebMD article listed above under datasets. In cleaning the 2018 data, we dropped unnecessary columns and renamed the columns to be more concise. Then, we had to extract the answers for screen time on the survey by creating a for loop. We then got the average and then plotted using matplotlib.

![IMG3](https://github.com/isabelleroet/tiktok/blob/f6b0056728c649d71ff33d8df1849d8cc870399c/tiktokimg/Screenshot%202023-03-27%20at%201.03.58%20AM.png) For graphing the global average screen time from 2022 to 2023, we passed the csv through a reader and dropped all the NA values to clean the dataset. We then sorted the data into ascending order. We then plotted the graph using matplotlib and set multiple colors for the bars.

![IMG4](https://github.com/isabelleroet/tiktok/blob/f6b0056728c649d71ff33d8df1849d8cc870399c/tiktokimg/Screenshot%202023-03-27%20at%201.06.26%20AM.png) For retrieving the weather in San Jose, San Francisco, and Berkeley: we created the query url with the API key and the units. We then created a list for the cities including San Jose, San Francsico, and Berkeley. We then created a for loop to to get the cities' latitude, longitude, and temperatures of the 3 cities from the API.

## Data Analysis
## TikTok Compared to Streaming Sites:

For all the streaming sites, they showed similar trends in the increase of revenue and users, where there is an increase in revenue and a significant increase in users/subscribers. These numbers are expected, due to the following factors:

First, at the height of the COVID-19 pandemic, the entire country was under lockdown for months. With the extended period of time indoors, people had to get creative on how to spend their time. The graphs will portray a significant increase in subscribers from 2019 to 2020, which is peak lockdown; and then a significant decrease from 2021 to 2022 when lockdowns eased. This corresponds with an increase in screentime, as more people are watching shows on different platforms.

Lastly, as the users/subscribers increased, the revenue for the companies also increased. The difference in severity can be explained due to the fact that users of streaming platforms tend to share accounts and costs, especially during the pandemic where majority of the population became unemployed. Nonetheless, the stock prices for these companies still had a significant increase from 2019 to 2020.

In the following section, we will be diving deeper into the numbers for the aforementioned streaming revenue and users for Netflix, Hulu, Twitch, YouTube, and finally TikTok.

## Netflix Revenue & Netflix Subscribers
![IMG5](https://github.com/isabelleroet/tiktok/blob/f6b0056728c649d71ff33d8df1849d8cc870399c/tiktokimg/Screenshot%202023-03-27%20at%201.04.10%20AM.png)
For Netflix, there was an average increase in subscribers of 27.8% pre-pandemic (2011 to 2018) and an inrease of 24% during the pandemic (2019 to 2020).

In terms of revenue, Netflix had an average increase of 25.2% pre-pandemic (2011 to 2018) and an increase of 17.1% during the pandemic (2019 to 2020).

## Hulu Revenue & Hulu Subscribers
![IMG6](https://github.com/isabelleroet/tiktok/blob/f6b0056728c649d71ff33d8df1849d8cc870399c/tiktokimg/Screenshot%202023-03-27%20at%201.04.30%20AM.png)
For Hulu, there was an average increase in subscribers of 39.5% pre-pandemic (2010 to 2018) and an inrease of 35% during the pandemic (2019 to 2020).

In terms of revenue, Hulu had an average increase of 35% pre-pandemic (2010 to 2018) and an increase of 19.30% during the pandemic (2019 to 2020).

## Twitch Revenue & Twitch Concurrent Viewers
![IMG7](https://github.com/isabelleroet/tiktok/blob/f6b0056728c649d71ff33d8df1849d8cc870399c/tiktokimg/Screenshot%202023-03-27%20at%201.04.40%20AM.png) 
For Twitch, there was an average increase in subscribers of 27% pre-pandemic (2016 to 2018) and an inrease of 68% during the pandemic (2019 to 2020).

In terms of revenue, Twitch had an average increase of 81% pre-pandemic (2016 to 2018) and an increase of 13% during the pandemic (2019 to 2020).

## YouTube Revenue & Youtube Premium Subscribers
![IMG8](https://github.com/isabelleroet/tiktok/blob/f6b0056728c649d71ff33d8df1849d8cc870399c/tiktokimg/Screenshot%202023-03-27%20at%201.04.46%20AM.png)
For YouTube, there was an average increase in premium subscribers of 116.82% pre-pandemic (2015 to 2020) and an inrease of 73.33% during the pandemic (2019 to 2020).

In terms of revenue, YouTube had an average increase of 40.67% pre-pandemic (2010 to 2018) and an increase of 33.24% during the pandemic (2019 to 2020).

## TikTok Revenue & TikTok User
![IMG9](https://github.com/isabelleroet/tiktok/blob/f6b0056728c649d71ff33d8df1849d8cc870399c/tiktokimg/Screenshot%202023-03-27%20at%201.04.51%20AM.png)
For TikTok, there was an average increase in premium subscribers of 145% pre-pandemic (2017 to 2019) and an inrease of 63.28% during the pandemic (2020 to 2021).

In terms of revenue, TikTok had an average increase of 135.5% pre-pandemic (2017 to 2019) and an increase of 292% during the pandemic (2020 to 2021).

## TikTok Followers
![IMG10](https://github.com/isabelleroet/tiktok/blob/f6b0056728c649d71ff33d8df1849d8cc870399c/tiktokimg/Screenshot%202023-03-27%20at%201.06.07%20AM.png)
TikTok's followers for popular users increased 394% from 2019 to 2020 and decreased 29.3% from 2020 to 2021.

## TikTok Shares and Comments

![IMG11](https://github.com/isabelleroet/tiktok/blob/f6b0056728c649d71ff33d8df1849d8cc870399c/tiktokimg/Screenshot%202023-03-27%20at%201.06.14%20AM.png)
Tiktok's shares and comments increased by 211.07% and 637.72% respectively. Tiktok's shares and comments decreased by 51.63% and 60.90% respectively. 

## TikTok Plays and Likes 
![IMG12](https://github.com/isabelleroet/tiktok/blob/f6b0056728c649d71ff33d8df1849d8cc870399c/tiktokimg/Screenshot%202023-03-27%20at%201.06.20%20AM.png)
Tiktok's plays and likes increased by 385.57% and 92% respectively. Tiktok's shares and comments decreased by 45.93% and 72% respectively. 

## Conclusion 
Based on the data we gathered and analyzed, we were able to infer the following conclusions:

First, there was a significant increase in both users and revenue between 2020 to 2021 across all the different social media platforms (Facebook, Hulu, Netflix, etc.), but TikTok succeeded way more than expected and that was boosted due to the pandemic. With everyone stuck at home during the lockdown, a lot of people had to pre-occupy themselves, which involved being on the computer a lot more. The internet became our connection to the “outside world” and a lot of school/work were also held online.

Directly from the first point, the second major conclusion is that there was a significant decrease come 2022 to 2023 because lockdown restrictions eased and people were able to spend their time somewhere else again. With schools and work also reverting from hybrid to back to the office settings, people have started spending less time online, which explains why there was a significant decrease.

Lastly, TikTok’s success is very interesting to note because compared to other well-established social media platforms, it is relatively younger. However, the impact of its success can be seen with other social media companies mimicking its algorithm. Examples of this include Facebook’s and Instagram’s reels, Snapchat’s Spotlight feature, and YouTube shorts.
