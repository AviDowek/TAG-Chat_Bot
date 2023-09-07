# TAG-Chat_Bot
This is a work in progress and an attempt to create a generative chatbot that is trained on the TAG Slack Channels and the Internal Wiki.     The training data currently is built
off of the Slack data which is scraped in a Dict format with questions being the key and answers being the value.       It will then be tokenized using BPE and converted to
sequences to enable it to be fed into a Neural Network for training.    The initial model will be an RNN and depending on it's performance, more models may be used.    

Current Contents:/n

1: Slack_Scraper:   This is a simple scraper that uses the Slack API to join channels and then scrape all data.   Data is not stored in a DICT format.  This was created at
an earlier stage of the project and is being retained for potential futures use in the project.

2: TAG_Scraper:    This is a simple Web Crawler and Scraper for scraping the TAG internal Wiki.  It functions by crawling and adding links to a list.  We then iterate through
the list and scrape the data.   Data is stored in a text file with headings for each topic.    The intended goal is to use Text Summerization on each entry and use the output
as part of the Bot Knowledge Base.

3:Slack_Dict:     This is a modified version of the Slack_Scraper that stores Questions and Answers in DICT format.


This page will be updated as the project progresses.
