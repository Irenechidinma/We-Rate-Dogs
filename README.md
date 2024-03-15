# We-Rate-Dogs Project 
# By Nwajagu Irene

The dataset that I worked on is the tweet archive of Twitter user @dog_rates, also known as WeRateDogs. WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. To make the dataset ready for analysis, I went through the following steps:

Data gathering

Data assessing

Data cleaning

Data Gathering

I worked with two datasets which are; twitter archive and the image prediction file. The twitter archive was gotten using the twitter API, this twitter API helped me to get additional information needed for the analysis which are the favorite count and each tweets retweet count.

# Data Assessing
After gathering the datasets, I performed a visual assessment which was done by opening the file on excel and scanning through it for any visible quality and tidiness issue,also I performed a programmatic assessment which was done by running some codes. These assessment lead to the discovery of the following issues:

The tweet_id column is duplicated as we have the same across the three dataframes used for the analysis
There is a html tag on the source column in the twitter archive enhanced data set.
In the image prediction table some breed names start with upper case while some are in lower case. there need to be some form of consistency.
In the twitter archive table the timestamp is in object datatype instead of datetime.
The tweet_id is in int64 instead of string data type
There are empty cells in the twitter archive enhanced file'
The in_reply_to_status_id, in_reply_to_user_id,retweeted_status_id, retweeted_status_user_id, retweeted_status_timestamp, img_num, p1, p1_conf, p1_dog, p2,p2_conf, p2_dog, p3, p3_conf, p3_dog will not be needed in this analysis.
The stages of dog should be in one colunm rather than seperate columns.
Some names in p1 are having _ and - which is not supposed to be.
Text and url are joined in one column
The above issues were resolved using the Define, code, and Test . After the cleaning process was completed I stored the cleaned data into a new file. The wrangling process was taken a step futher to discover some key insights.
