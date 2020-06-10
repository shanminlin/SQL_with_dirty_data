# SQL with dirty data

Here I'm working with data to do some user segmentation analysis based on their geographics and actions.
The challenge is that in the data, columns with duplicate values are used to link tables together. Therefore, we need to be careful when doing joins as duplicate rows in these columns can lead to multiplication of duplicate rows. Moreover, in the 'users' and 'dogs' tables, there is a field named 'exclude', which indicates whether a particular user ID or dog ID should be excluded in our analysis. Only those user/dog IDs with 'exclude' equal to 0 or missing should be included. 

Acknowledgement:
- The dataset is from "Managing Big Data with MySQL" course from Coursera.
