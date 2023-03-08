# reddit_nlp_analysis
# Portfolio Project: Reddit BJJ Data Analysis

This project is a Python script that extracts data from the Reddit API, cleans and analyzes the data using NLP techniques, and performs sentiment analysis on the text. The purpose of this project is to analyze the sentiment of posts related to Brazilian Jiu-Jitsu (BJJ) and identify the most frequently mentioned people and topics. A dashboard is also being developed to link to the output csv and images, a quick basic plan view can be seen below:

![Sample dashboard](https://user-images.githubusercontent.com/68299933/223722503-bc2a5c99-4435-4f06-99c3-96de4665840f.jpg)

### Libraries Used:
- requests
- pandas
- nltk
- spacy
- numpy
- selenium
- urllib
- PIL
### Getting Started
Clone this repository to your local machine.
Create a virtual environment and activate it.
Install the required libraries using pip install -r requirements.txt.
Create a Reddit account and obtain API credentials from the Reddit API.
Add your credentials to secret.txt, pw.txt, and user.txt.
Run the script.

### Using the Script
When the script is run, it will first obtain authorization to access the Reddit API using the credentials provided in secret.txt, pw.txt, and user.txt. It will then extract the 100 most recent posts from the BJJ subreddit.

The script will clean the data by removing stop words and extracting names using the spacy library. It will then perform sentiment analysis on the text using the nltk Sentiment Intensity Analyzer.

The script will output a DataFrame containing the names of people mentioned in each post and the positive words used in each post. The DataFrame will be saved to a CSV file called bjj_sentiment_analysis.csv.

### Output
The output of the script is a CSV file called bjj_sentiment_analysis.csv. This file contains the following columns:

names: a list of the names mentioned in the post.
positive_words: a list of the positive words used in the post.
Note
This project is limited to analyzing the sentiment of posts related to BJJ on Reddit. It is not intended to provide any conclusive analysis of the community or the sport.



