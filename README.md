# 10-K Insights: Sentiment Analysis and Stock Returns for S&P500 Stocks in 2022

Nicole ElChaar, FIN337, Spring 2023

## Summary

In this analysis, we explore whether 10-K filings contain value-relevant information in the sentiment of the text.  We examine the relationships between sentiments found in 10-K filings and returns following the 10-K's release using two valence-based dictionaries and three topic-based schemes (with financial stability, corporate governance, and e-commerce themes).  We find higher absolute correlations for positive sentiments in general, with the largest magnitudes for positive e-commerce topics, positive LM sentiment, negative LM sentiment, and positive financial stability topics.

The final output is *output/analysis_sample.csv* which includes the following:

1. 5 positive sentiment scores
1. 5 negative sentiment scores
1. a return variable from the day of the 10-K's release to two days following
1. a return variable from two days after the 10-K's release to ten days following 
1. the 10-K's word count
1. the 10-K's unique word count
1. accounting variables for further analysis

## Requirements

Python, Jupyter Notebook, and the following Python packages are required:

- glob
- os
- re
- pandas
- bs4 (BeautifulSoup)
- tqdm
- zipfile
- urllib
- io
- requests_html
- time
- import matplotlib
- seaborn
- statsmodels
- warnings
- sec_edgar_downloader

## Usage

**⚠️⚠️⚠️WARNING⚠️⚠️⚠️ The files contained in this code will download up to 10GB of data.  Please keep this in mind before continuing**

First, run all lines in the *download_text_files.ipynb* notebook to gather necessary filings and returns.  Then, build the sample with *build_sample.ipynb*.

An existing analysis is shown in *report.ipynb*.

## Key Input Files

Input files are described in more detail in *inputs/README.md*.

## References

<a id="1">[1]</a>
Correa, Ricardo, Keshav Garud, Juan-Miguel Londono-Yarce, Nathan Mislang (2017). "Constructing a Dictionary for Financial Stability." IFDP Notes. Washington: Board of Governors of the Federal Reserve System, June 2017, https://doi.org/10.17016/2573-2129.33.

<a id="2">[2]</a>
Diggelmann, Thomas, Jordan Boyd-Graber, Jannis Bulian, Massimiliano Ciaramita, Markus Leippold (2020). "CLIMATE-FEVER: A Dataset for Verification of Real-World Climate Claims." Tackling Climate Change with Machine Learning workshop at NeurIPS 2020, 11 December 2020.

<a id="3">[3]</a>
Goodell, John W, Satish Kumar, Weng Marc Lim, Debidutta Pattnaik (2021).
"Artificial intelligence and machine learning in finance: Identifying foundations, themes, and research clusters from bibliometric analysis."
Journal of Behavioral and Experimental Finance, Volume 32, https://doi.org/10.1016/j.jbef.2021.100577.

<a id="4">[4]</a>
Mushtaq, Rizwan, Ammar Ali Gull, Yasir Shahab, Imen Derouiche (2022), "Do financial performance indicators predict 10-K text sentiments? An application of artificial intelligence," Research in International Business and Finance, Volume 61, 2022. https://doi.org/10.1016/j.ribaf.2022.101679.

<a id="5">[5]</a>
Shea, Yifei, Margit Steiner, Erhard Radatz (2021). "Sustainable Investing Meets Natural Language Processing - a Systematic Framework for Building Customized Theme Portfolios". Risk & Reward, Volume 3/2021, pp. 4-13., https://ssrn.com/abstract=3909330.
