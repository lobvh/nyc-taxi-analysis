# nyc-taxi-analysis

![alt text](https://productplacementblog.com/wp-content/uploads/2021/06/Manolo-Blahnik-Store-Paper-Bag-Held-by-Sarah-Jessica-Parker-as-Carrie-Bradshaw-in-Sex-and-the-City-S04E12-1-1536x864.jpg)

This project was first meant to serve as a playground to learn Apache Spark by exploring its various functionalities and understanding the theory behind it, but furthermore scaled to analysis project since some excercises *sparked* (get it?) my interest to further investigate and understand the data. 

NYC Taxi data is a collection of all the trips done in February / 2021. In one of the excercises I had to calculate the "the most common pickup-dropoff pair" and it turns out that it is the one occured in the same zone of NY:

+------------+------------+---------+
|PULocationID|DOLocationID|frequency|
+------------+------------+---------+
|          76|          76|    45041|
|          26|          26|    37329|
|          39|          39|    28026|
|          61|          61|    25976|
|          14|          14|    17934|
+------------+------------+---------+

I just had to further investigate it, and found out that only three vehicles in the New York (for that month being!) contributed to the case of driving in the same NY zones:

+-----------------+---------+
|hvfhs_license_num|frequency|
+-----------------+---------+
|           HV0003|   648406|
|           HV0005|   245014|
|           HV0004|     2788|
+-----------------+---------+

which, apart from other facts that I've discussed in the notebook, led me to the conclusion that on average most people churned their trips in those taxi cabs in no more than 10mins! 

There are around 900k such trips in just one month, and as a taxi service this kind of analysis would help in further investigating what happend and see if it potentialy harms my income. Maybe it is because of high traffic congestion in NY and people decide it is better to walk? Maybe this analysis would help to re-route some taxi cabs in those areas? 
