# Wrangle & Cleaning of WeRateDogs
### Introduction

The dataset wrangles in this project is the tweet archive of Twitter user @dog_rates, also known as WeRateDogs. It rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10. The numerators, though? Almost always greater than 10. (11/10, 12/10, 13/10). 

### Gathering Data
The data is gathered from different sources and finally merged to analyse and visualize the data.
+ **Twitter archive file**
Twitter archive contains basic tweet data for all 5000+ of their tweets, but not everything. One column the archive does contain though: each tweet's text, which I used to extract rating, dog name, and dog "stage" (i.e. doggo, floofer, pupper, and puppo) to make this Twitter archive "enhanced." Of the 5000+ tweets, I have filtered for tweets with ratings only (there are 2356). The file is named as **twitter-archive-enhanced.csv**

+ **Tweet Image prediction**
This file contains top 3 predictions of for each dog image from the twitter archive file. Data is downloaded from the URL provided by the Udacity using the request library and loaded into **image-predictions.tsv**. This data consist of 2075 rows and 11 columns 

+ **Twitter API file**
The file contains tweet id, favorite count and retweet count. Data has downloaded manually **(tweet-json.txt).** This data consist 2354 rows and 2 columns.

### Assessing Data
After the data has been gathered it is assessed to find the Null values, missing
values and inapproriate measure or data entry. For detailed report on assessing the data please refer to **wrangle_report.pdf**

### Conclusion
+ **Top breeds rated by WeRateDogs** - <font size= 14> On analysis we found that </font> **Golden Retriver** is the most common breed rated by the WeRateDogs followed by Labrador Retiver, Pembroke, and Chihuahua.  

+ **Most popular category** - WeRateDogs classified dogs as Doggo, Pupper, Floofer and, Puppo. Most of the dogs rated by this twitter account comes under **Pupper** category.  

+ **Most retweeted dog and its like** -The most retweetd dog was **Labrador Retiver 79515 retweets** and **131075 favourite** by people.   

+ **Account Popularity** - The page gained popularity over time. There is an **upward trend in the number of favorites** which is an evidence of account is getting popular among thepeople.
