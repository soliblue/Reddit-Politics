## A Characterization of Political Communities on Reddit
This repository contains the code and results of our paper "A Characterization of Political Communities on Reddit".

1. In order to run the code you need to download the Reddit data first. The data can be downloaded from: https://files.pushshift.io/reddit/
2. The path for the downloaded data should then be updated in all notebooks. 
3. The result files were compressed using gzip in the terminal.
4. Before running the notebook in 00_General you need to run all notebooks in 01_Content_Analysis/PreProcessing

### Required Libraries
* numpy
* fastText
* nltk
* plotly
* matplotlib
* gzip
* pickle

### Results

The results are stored in two folders.

**Files > 100MB are only available on google drive: https://drive.google.com/drive/folders/1VetvLETa-9_jao9ihAtZjwvc4ofI8xrO?usp=sharing.**

- **Plots**: The plots folder contains the plots and tables generated.
- **Results**: The Results folder contains the results of the calculations.
  - Links
    * **comment_links.pickle.gz** 
      + stores information about the frequencies of all top level domains posted on the studied subreddits.  
      + **Example**: comment_links['The_Donald'] returns all domains posted on The_Donald alongside their frequency. 
      + This is a Counter object so one can type comment_links['The_Donald'].most_common(100) to get the top 100 shared domains. 
    * **comment_full_links.pickle.gz** 
      + stores information about the frequencies of each link posted on studied subreddits.  
      + **Example**: comment_full_links['politics'] returns all links posted on politics alongside their frequency. 
      + This is a Counter object so one can type comment_links['politics'].most_common(100) to get the top 100 shared domains. 
  - Word Frequencies
    * **word_freq.pickle.gz** 
       + stores information about the relative count of all words posted on the studied subreddits.  
       + **Example**: word_freq['The_Donald'] returns all words posted on The_Donald alongside their frequency. 
       + This is a Counter object so one can type word_freq['The_Donald'].most_common(100) to get the top 100 shared words. 
     * **word_freq_unique.pickle.gz** 
       + stores information about the relative diff count of all words posted on the studied subreddits.
  - Sentiment 
    * **sentiment_The_Donald.pickle.gz**: contains sentiment score for all comments posted on The_Donald
    * **sentiment_politics.pickle.gz**: contains sentiment score for all comments posted on politics
    * ...
    * **sentiment_altright.pickle.gz**: contains sentiment score for all comments posted on politics
  - WordEmbeddings
    * We have the word embeddings for all studied subreddits. 
  - Subreddit Embeddings
    * We have subreddit embeddings calcualted as described in this article: https://fivethirtyeight.com/features/dissecting-trumps-most-rabid-online-following/. 

**Remarks** 
- We are still cleaning the code and results to make it easier to understand and reuse. 
