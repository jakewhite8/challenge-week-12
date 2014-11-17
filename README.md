# Challenge Week 12 Submission Template
Jake White
# Reddit Data Challenges

## Challenge 1

![image](http://i.imgur.com/dwn5aQE.png)

## Challenge 2

there are over 12,000,000 data points, which I assume are individual comments, which is very interesting considering the data was collected over only two weeks

![image](http://i.imgur.com/I0CLesK.png)

## Challenge 3

each node has a field which indicates the subreddit it is attached to. with this information we can learn which subreddit communities are most active. for example the "leagueoflegends" community had over 310,000 posts within the two week period

![image](http://i.imgur.com/PFVda0D.png)

## Challenge 4

you could examine each comment for key words and from that you could come to a conclusion regarding the majority of the reddit commentors general tones and learn from this about the reddit community as a whole

## Challenge 5

[Link to Code or pasted code]
[Answer]

## Challenge 6

users with unpopular opinions would be outcast from the data analysis 

## Challenge 7

users with popularly viewed comments would only be accounted for, so the conclusion is not nessisarily accurate because not all authors are being accounted for, so yes my conclusions on the data would be changed

## Challenge 8

we are only looking at the top 50 subreddits, when there exists many other subreddits that may more closely share active commentors


## Challenge 9

the data we are examining is only over a two week period, so it may be bias in that one subreddit may not have been actively commenting for whatever reason over this time period and therefore the conclusions as to which groups share the most commentors is not accurate

## Challenge 10

you can re-examine the data given a larger time period (larger than two weeks/ different two weeks), you could also expand the number of subreddits included in the domain of subreddits being tested for similarity (more than the top 50)

# Yelp and Weather 

## Challenge 1

db.precipitation.aggregate([{$match: {"date": /20100425.*/}},{$match: {"station.name": "MADISON DANE CO REGIONAL AIRPORT WI US" }},{$group:{_id: null, total: { $sum: "$hpcp"}}}]);

Answer: 62

![image](http://i.imgur.com/R5ZNs5Q.png)

## Challenge 2

db.normal.aggregate([{$match: {"DATE": /20100425.*/}},{$match: {"STATION_NAME": "LAS VEGAS MCCARRAN INTERNATIONAL AIRPORT NV US" }},{$group:{_id: null, average_windspeed: { $avg: "$HLY-WIND-AVGSPD"}}}]);

Answer: 110.08333333333333

![image](http://i.imgur.com/KnVJm6u.png)

## Challenge 3

db.business.aggregate([{$match : {"city": "Madison"}},{$group:{_id:null, total_reviews:{$sum:"$review_count"}}}]);

Answer: 34,410

![image](http://i.imgur.com/Rjo7TkI.png)

## Challenge 4

db.business.aggregate([{$match : {"city": "Las Vegas"}},{$group:{_id:null, total_reviews:{$sum:"$review_count"}}}]);

Answer: 577,550

![image](http://i.imgur.com/XMD0SbN.png)

## Challenge 5

db.business.aggregate([{$match : {"city": "Phoenix"}},{$group:{_id:null, total_reviews:{$sum:"$review_count"}}}]);

Answer: 200,089

![image](http://i.imgur.com/pM19HXv.png)







