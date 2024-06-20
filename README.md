# Twitter-Data-Analysis---SQL-Project
Performed Data Analysis on Twitter Data in Databricks SQL (Community Edition)

The project was submitted as a solution to one of my coursework challenges- 2023-24 CST4070 Applied Data Analytics - Tools, Practical Big Data Handling, Cloud Distribution

### SQL Concepts Utilised:
1. Aggregate Functions (SUM, AVG, MIN, MAX, COUNT)
2. Joins
3. Window Functions ( ROW_NUMBER(), RANK(), DENSE_RANK() )
4. Common Table Expressions (CTE) using WITH clause
5. Filtering using WHERE and HAVING clauses
6. Ordering using ORDER BY clause
7. Pattern identification and analysis using LIKE keyword
8. CASE WHEN statements
9. Table and column Aliases
10. Relational and Arithmetic Operators
### Flow of Analysis:
#### Dataset Preparation
Imported the followers, users and tweets tables. \
Note: The datasets are not real Twitter data. The simulated datasets were provided by the university for the purpose of the coursework. \
Created follower_count table from followers tables, to get information about the number of followers for each user. 
### FOLLOWER ANALYSIS:
1. Users with the highest number of followers
2. Follower count statistics (min, max, avg) by age group
3. Top 5 users in each age group with the highest number of followers
4. Users who follow back all their followers and their proportions
5. Whether young or older users generally follow users in their same age group
6. Top 10 most active users per age group
### TWEETS ANALYSIS:
7. Total tweet count and average tweet count by age group. Percentage by which young people tweet more.
8. Proportions of total tweets with and without hashtags and by age group
9. Comparison of tweet lengths between young and old users
10. Longest and shortest tweet and the corresponding users
11. Tweets with funny sentiment (lol, haha, hehe, rofl, hahaha) and their distribution among different age groups
12. Proportion of tweets containing questions
13. Ratio of tweets containing links for different demographics
14. Top 10 most common words used in tweets and the age group that used these words
15. Top 10 most mentioned users in tweets
### HASHTAGS ANALYSIS:
16. Top 10 hashtags (overall)
17. Popular hashtags among young users
18. Popular hashtags among old users
19. Most popular hashtags per day of the week
20. Most popular hashtags by month
### TEMPORAL ANALYSIS:
21. Monthly tweet volume trends by age group
22. Comparison of tweet activity on weekdays vs weekends among different demographics
23. Most active hour for tweeting by age group
24. Average number of tweets per week by age group
25. Most active days for users with the highest followers

### Insights from Analysis:
1. Five users are tied in the first spot for the highest number of followers, with 11 followers.
2. The average number of followers for young people is 4, which is slightly greater than the average number of old people, which is 3.
3. Only 16.61% of users follow back all their followers. i.e. 5181 users follow back all their followers, out of a total of 31185 users.
4. People prefer following their own age group people more (old-old = 33771, young-young = 62217). However, old people follow more young people, than young people following old people. i.e. 6125
old people follow young people. Whereas, only 2555 young people follow old people.
5. Young users (18003) tweet approximately 36.24% more than old users (13214).
6. Overall, only 4.09% of tweets had hashtags. The proportion of tweets that had hashtags were more in young people than old. Only, 2.57% of tweets used by old people had hashtags. In comparison,
5.22% of tweets used by young people had hashtags.
7. On an average, old people’s tweets were longer (tweet length : 94) than young people (tweet length : 90).
8. The longest tweet belonged to user ShayMarie09 and the shortest tweet belonged to user yoyoskittles.
9. Young people tweet funny content more than twice as often as old people, indicating a strong preference for humor among younger users.
10. 9.96% of the total tweets contain questions. This indicates that a significant portion of users' tweets are intended to engage others, spark conversations, or seek information and feedback.
11. Young users include links in their tweets at a higher rate (6.57%) compared to older users (4.22%). This indicates that younger users are more likely to share external content, references, or promotional
materials through their tweets.
12. In the most common words used in tweets, the words "music", "movies", and "love” suggests that younger users are likely to tweet about their personal interests, hobbies, and feelings. The words
"family" suggests that older users may prioritize tweeting about their personal life and family-related topics.
13. Most of the top mentioned users are music artists or related to the music industry, indicating that music-related content is highly engaging on this platform.
14. Top mentioned hashtags shows the communities interest in music (#musicmonday), social engagement (#followfriday, #fb) and global events (#iranelection).
15. The hashtags popular among young people show their heavy interest in music (#music, #music4good). The hashtags popular among old people (#travel, #traveltuesday, #knitting) show their interest in
travel, knitting and family.
16. Specific hashtags dominate particular days, like #musicmonday on Mondays and #followfriday on Fridays, suggesting thematic social media activities that users participate in.
17. The increasing use of #musicmonday from April (8) to June (300) suggests growing engagement with this hashtag over these months.
18. Both age groups show increasing tweet activity from April to June, with young users consistently tweeting more than older users. June shows the highest tweet activity for both age groups, indicating a
potential seasonal peak in user engagement.
19. Young users are more active on both weekdays and weekends compared to older users, with a significant number of tweets on weekdays.
20. Weekend vs. Weekday Activity: Young users' tweet volume decreases by 15.68% on weekends, while older users' tweet volume only decreases by 2.22%, indicating that older users maintain a more
consistent tweeting pattern throughout the week.
21. Young users are most active at night (10PM), while older users are most active early in the morning (6AM), reflecting different daily routines and peak engagement times.
22. Users with the highest followers are most active on weekends, particularly Sunday, suggesting that weekends are a prime time for engagement. There's still significant activity on other days like Tuesday.

### I was able to successfully draw meaningful insights from the datasets, by joining multiple tables, using SQL queries in Databricks Community Edition.
