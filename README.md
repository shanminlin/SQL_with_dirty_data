# Data-Analysis-with-SQL

My goal for this project is to demonstrate how to conduct a data analysis project using SQL.
![alt text](http://url/to/img.png)

# 1. Business issue identification
Dognition is a company that teaches users how to build a deeper connection with their dogs. 
Users will pay for playing 20 games with their dogs for assessing 5 core dimensions of cognition for their dogs: empathy, communication, cunning, memory, and reasoning. With a few exceptions, all games are presented to customers in the same order. Customers are not able to advance through tasks or trials out of order. When users finish the assessment, they will receive a 10-15 page report about their dogs’ unique personality dimension. After completing the 20-game Dognition Assessment, customers can sign up to receive additional games and activities at the rate of one game and one activity per month. The company aims to collect as much data as possible from as many different kinds of dogs as possible. So they want to figure out what business changes they could implement to increase the number of tests that users complete on their website. The dataset is from "Managing Big Data with MySQL" course from Coursera.

# 2. Project scope
Goal: Our goal is to help the company assess which users and when it should target for promotions, encouragement messages and remainders etc. for increasing number of tests completed.
Analysis: We will conduct user segmentation analysis based on users' geographics and behavioral tendencies, as well as their dogs' information.

# 3. Key challenges
We notice that none of the Dognition tables have primary keys declared. Instead, the "MUL" in the "Key" column will be used to link tables together. Note that as these fields are not primary keys, they may contain duplicate values. Therefore, we need to be careful when doing joins as duplicate rows in the columns that are use for joining tables can lead to multiplication of duplicate rows. Moreover, in the 'users' and 'dogs' tables, there is a field named 'exclude', which indicates whether a particular user ID or dog ID should be excluded in our analysis. Only those user/dog IDs with 'exclude' equal to 0 or missing should be included. 
