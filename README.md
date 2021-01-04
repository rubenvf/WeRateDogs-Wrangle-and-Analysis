# WeRateDogs-Wrangle-and-Analysis
Code for project 4 Udacity's Data Analyst Nanodegree

Real-world data doesn't usually come clean, so the aim of this project is to collect, assess and clean up three dataframes associated with the [WeRateDogs Twitter account](https://twitter.com/dog_rates?ref_src=twsrc%5Egoogle%7Ctwcamp%5Eserp%7Ctwgr%5Eauthor).

#Data

- `twitter-archive-enhanced.csv`: This document was delivered directly by Udacity and downloaded manually. It contains the following columns: tweet_id ,in_reply_to_status_id, in_reply_to_user_id, timestamp source, text, retweeted_status_id, retweeted_status_user_id, retweeted_status_timestamp, expanded_urls, rating_numerator and rating_denominator.

- `image_predictions.tsv`: This file is located on a Udacity server and was downloaded through its url. It contains information related to a neural network classifier of dog breeds. Its columns are: tweet_id, jpg_url, img_num, p1, p1_conf, p1_dog, p2, p2_conf, p2_dog, p3, p3_conf and p3_dog.

- `tweet_json.txt`: This information was obtained by communicating with the Twitter API. It shows the quantification of retweets and favourites for each tweet. Its columns are: tweet_id, retweet_count and favorite_count.

# Analysis

The analysis has been carried out in 3 different documents:

- `wrangle_act`: The whole code of this project is developed in this file, which has been carried out in a Jupyter Notebook. It has four different points: Gathering, Assess, Clean and Analysis. | [Preview](https://github.com/rubenvf/WeRateDogs-Wrangle-and-Analysis/blob/main/wrangle_act.ipynb)

- `act_report`: Report framed as a blog post to show to the general public. | [Preview](https://github.com/rubenvf/WeRateDogs-Wrangle-and-Analysis/blob/main/act_report.pdf)

- `wrangle_report`: Report framed as an internal file to document the efforts made in the data wrangling process. | [Preview](https://github.com/rubenvf/WeRateDogs-Wrangle-and-Analysis/blob/main/wrangle_report.pdf)

# Conclusion

- **Insight 1: The dogs in the stage pupper have the highest number of tweets.**

- **Insight 2: According to the neural network classifier, the most published breed of dog is the golden retriever, followed by labrador retriever and pembroke.**

- **Insight 3: The data shows that the favorite dog stage is the puppo one, as it has a greater number of both, retweets and favourites, closely followed by the doggo stage. As for the rating given by the WeRateDogs Twitter account, the only stage with a different median rating is the puppy stage, with an median of 1.1. The other 3 stages, doggo, puppo and floofer, have a median of 1.2.**

- **Insight 4: The vast majority of tweets from the WeRateDogs account, 93.6%, have been made from the Twitter App for iPhone.**

- **Insight 5: More than half of the tweets on the account, 51.3%, have been posted between 0 am and 6 am and between 6 am and 12 pm, only 0.2% of the tweets have been posted.**

- **Insight 6: The peak month is December and the off-peak month is August.**

- **Insight 7: The French bulldog is the dog breed with the greatest confidence in prediction although confidence is at its highest when the image is a screenshot, since the classifier categorises it as a web site.**

- **Insight 8: The neural network classifier is more efficient in predicting whether or not an image corresponds to a dog, when it receives images of the most published breeds, with a 94.5% success rate. In the case of prediction in general, this efficiency drops to a 73.8% success rate.**
