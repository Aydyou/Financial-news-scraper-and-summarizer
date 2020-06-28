# Financial news scraper and summarizer

 This app scrapes financial news, summarizes them and gives them a sentiment score.
You need the latest pytorch with gpu support, transformers, bs4 and flask to be able to run it. So be sure install them beforehand. The app utilizes the Huggingface summarizer based
on Bart to summarize the scraped data from news media. Then uses the Vader sentiment analyzer to give it a score. The score is calculated between 0 and 100.

 By default the summarizer pipeline will utilize your gpu. If you do not have gpu support please the "device" parameter from the pipeline. 
 
 For scraping news from nytimes, we are using a free account for logging in. I've removed my login information, so please add yours at XXXXX place holders.
 
 Each time you click the Get Sentiment button it brings 20 summarized news with averaged sentiment score. (Each time score is average with all previous clicks). The maximum number of 
links that you can scrape is about 150 news article and the totaling number of characters of all news is about 1 million characters. The summarizer compresses this to a character number
between 70 and 80 thousands. 

