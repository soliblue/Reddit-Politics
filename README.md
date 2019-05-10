### A Characterization of Political Communities on Reddit

This repository contains the code and results of our paper "A Characterization of Political Communities on Reddit".


#### Results
The results can be found in the folder Results or on google drive (https://drive.google.com/drive/folders/1VetvLETa-9_jao9ihAtZjwvc4ofI8xrO?usp=sharing). Files > 100MB are only available on google drive. 

- Links
  * **comment_links.pickle.gz** 
    + stores information about the frequencies of all top level domains posted on the studied subreddits.  
    + **Example**: comment_links['The_Donald'] returns all domains posted on The_Donald alongside their frequency. 
    + This is a Counter object so one can type comment_links['The_Donald'].most_common(100) to get the top 100 shared domains. 
  * **comment_links.pickle.gz** 
    + stores information about the frequencies of each top level domains posted on studied subreddits.  
    + **Example**: comment_links['The_Donald'] returns all domains posted on The_Donald alongside their frequency. 
    + This is a Counter object so one can type comment_links['The_Donald'].most_common(100) to get the top 100 shared domains. 
  
- Word Frequencies
  * **word_freq.pickle.gz** 
     + stores information about the relative count of all words posted on the studied subreddits.  
     + **Example**: word_freq['The_Donald'] returns all words posted on The_Donald alongside their frequency. 
     + This is a Counter object so one can type word_freq['The_Donald'].most_common(100) to get the top 100 shared words. 
   * **word_freq_unique.pickle.gz** 
     + stores information about the relative diff count of all words posted on the studied subreddits.  

**Remarks** 
- We are still cleaning the code and results to make it easier to understand and reuse. 
