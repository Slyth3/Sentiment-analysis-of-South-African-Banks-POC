# Bank Sentiment analysis
This project is to prove the concept of scraping the required tweets, use an out-the-box model to determine sentiment of tweets and visualize/analyse the results

Process: 
* Twint to scrape tweets of the top 4 banks in South Africa 
  Twint (https://github.com/twintproject/twint) 
* Clean tweets with WordPunctTokenizer and Regex 
* TextBlog to process sentiment of tweets 
* Matplotlib / Seaborn to visualise data 

Any tweets referencing the top 4 South African banks are scraped and their sentiment scored as eeher postive, neutral or negative:
  - Standard bank
  - Absa
  - Nedbank
  - FNB

Outfiles can be found on AWS S3 (as pickle files:
* pre-cleaned file (https://twint-nlp-banks.s3.eu-west-1.amazonaws.com/Output/Bank-NLP/Output/pre_cleaning.pickle)
* pre-cleaned CSV file (https://twint-nlp-banks.s3.eu-west-1.amazonaws.com/Output/Bank_NLP/Output/pre_cleaning.csv)
* Final output, cleaned and with sentiment analysis (https://twint-nlp-banks.s3.eu-west-1.amazonaws.com/Output/Bank_NLP/Output/Final.pickle)
