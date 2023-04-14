# BT4222_G1_Emoji_Recommendation_System
linked to google drive (with datasets used): https://drive.google.com/drive/folders/1-NNp2flaBTl217nvQK2TrtqnbXHFbhr9?usp=share_link

## Order of code flow:

Raw data from kaggle : 
`Kaggle_tweets.csv`
--filter by--> `Kaggle Data Filtering and Split Emoji.ipynb` 
--output--> `kaggle_tweets 15 selected emoji.csv`

Raw data from Twitter : 
`Twitter Scrapping.ipynb`
--output--> `tweets from scraping (batch x).csv`
--preprocess by--> `Scraped Data Processing (replicate tweets and remove skin-tone).ipynb` 
--output--> `preprocess_data.csv` ( & `preprocess_data_batch2.csv` after more scraping work was done)


`kaggle_tweets 15 selected emoji.csv` & `preprocess_data.csv`
--combine, clean, preprocess, split by--> `Text Cleaning and Preprocessing.ipynb`
--output--> `train 15 emoji.csv`, `test 15 emoji.csv`

`train 15 emoji.csv`, `test 15 emoji.csv`
--input to all codes for classification models
