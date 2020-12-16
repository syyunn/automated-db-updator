### Components: Abstract

1. API (Data) Provider 
2. Our Server system (Mostly RDBMS)

2-1. Data Schema To be Updated/Added 

2-1-1. W/ Certain Interval

### Component: Actual Frameworks To Use

0. Let current time point c, where c is represented as discrete time series, thus c \in \Bbb N
1. For every given time interval \i, AWS Lambda L runs.
2. L is defined as L: c -> retrieved_data for the period of time [c-1, c]
3. Then U, the updator implemented as AWS Lambda, updates the L(c) to the Database D.


### Detailed Steps:

#### Data Availability
1. create a Labmda that fetches bulk-data-availibity and saves the data into S3
