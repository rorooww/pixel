# pixel
pixel bounty
import tweepy

consumer_key = "YOUR_CONSUMER_KEY"
consumer_secret = "YOUR_CONSUMER_SECRET"
access_token = "YOUR_ACCESS_TOKEN"
access_token_secret = "YOUR_ACCESS_TOKEN_SECRET"

auth = tweepy.OAuthHandler(consumer_key, consumer_secret)
auth.set_access_token(access_token, access_token_secret)

api = tweepy.API(auth)

tweets = tweepy.Cursor(api.search_tweets, q="#wenpixel", since_id="OFFICIAL_PIXELS_ACCOUNT_ID").items()

for tweet in tweets:
    print(tweet.text)

>>>

import time
import subprocess

while True:
    subprocess.call(["python", "your_scraper_script.py"])
    time.sleep(900) # sleep for 15 minutes

>>>

import requests

url = "https://pixels-data.xyz/wen"
payload = {"twitter_id": "USER_TWITTER_ID", "tweet_id": "TWEET_ID"}
headers = {"Content-Type": "application/json"}

response = requests.post(url, json=payload, headers=headers)

print(response.status_code)

>>>

Test the responsive in twitter account
