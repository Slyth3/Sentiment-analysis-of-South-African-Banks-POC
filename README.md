# Bank Sentiment analysis
Sentiment Analysis on the top 4 banks in South Africa 
  - Standard bank
  - Absa
  - Nedbank
  - FNB

Process: 
* Twint to scrape tweets of the top 4 banks in South Africa 
  Twint (https://github.com/twintproject/twint) 
* Clean tweets with WordPunctTokenizer and Regex 
* TextBlog to process sentiment of tweets 
* Matplotlib / Seaborn to visualise data 

Outfiles can be found on AWS S3 (as pickle files:
* pre-cleaned file (https://twint-nlp-banks.s3.eu-west-1.amazonaws.com/Output/Bank-NLP/Output/pre_cleaning.pickle)
* pre-cleaned CSV file (https://twint-nlp-banks.s3.eu-west-1.amazonaws.com/Output/Bank-NLP/Output/pre_cleaning.csv)
* Final output, cleaned and with sentiment analysis (https://twint-nlp-banks.s3.eu-west-1.amazonaws.com/Output/Bank-NLP/Output/Final.pickle)
