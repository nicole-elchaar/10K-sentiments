# About these datasets

## *ML_negative_unigram.txt* and *ML_positive_unigram.txt*

_ML_ stands for "Machine Learning". 

These datasets are lists of words identified as having positive and negative sentiment in "The colour of finance words" (JFE, 2023).

- Citation: Garcia, Diego, Xiaowen Hu, and Maximilian Rohrer. "The colour of finance words." Journal of Financial Economics 147.3 (2023): 525-549.
- The paper is in the literature folder ("ML_JFE.pdf")
- Data downloaded from data availability section of [article webpage](https://www.sciencedirect.com/science/article/pii/S0304405X22002422#refdata001a)

## *LM_MasterDictionary_1993-2021.csv*

_LM_ stands for the names of the authors. 

Use this dataset to find the lists of words identified as having positive and negative sentiment by Tim Loughran and Bill McDonald. 

- Positive (negative) sentiment words have a strictly positive value in the positive (negative) column 
- Citation: Tim Loughran and Bill McDonald. "When is a Liability not a Liability? Textual Analysis, Dictionaries, and 10-Ks." Journal of Finance 66:1 (2011): 35-65. 
- The paper is in the literature folder("LM_JF.pdf")
- Data downloaded from https://sraf.nd.edu/loughranmcdonald-master-dictionary/, modified slightly for this midterm

## *s&p500_2022.csv*

This dataset lists tickers, CIKs, sectors, and other information about S&P500 companies.  It was originally downloaded from Wikipedia in early 2023.

## *topic_list.csv*

This file includes a list of terms included in the sentiment analysis of *build_sample.ipynb*.  Neutral topics are listed under type as <topic abbreviation>_topic, positive words are listed under type as <topic abbreviation>_positive, and negative words are listed under type as <topic abbreviation>_negative.  All terms are then listed to the right under term.

To add a list related to Customer Satisfaction, for example, add CSV data to the bottom of the file with general topics as "cs_topic,<term>", positive related words as "cs_positive,<term>", and negative related words as "cs_negative,<term>".  