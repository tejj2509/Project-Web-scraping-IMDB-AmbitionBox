# Web Scraping

Web scraping using the Beautiful Soup package is a powerful technique in the field of web data extraction and parsing. Beautiful Soup is a Python library that makes it easy to scrape and navigate through HTML and XML documents, extracting specific information from web pages. 

It is commonly used for various purposes, such as data collection, web content analysis, automation of repetitive tasks, and more. Beautiful Soup provides a convenient way to search, filter, and manipulate the elements of a web page, allowing you to extract structured data from unstructured web content.

The key features of Beautiful Soup include:

1. **Parsing HTML and XML:** Beautiful Soup parses HTML and XML documents and creates a parse tree, making it easy to navigate and extract data from web pages.

2. **Search and Navigation:** You can search for elements by tag name, attributes, or text content, and navigate through the document's structure.

3. **Data Extraction:** Beautiful Soup allows you to extract specific data points, such as text, links, images, and more from a web page.

4. **Robustness:** It handles malformed HTML gracefully, making it suitable for scraping websites with varying degrees of markup quality.

5. **Integration:** Beautiful Soup is often used in conjunction with other libraries, such as Requests for making HTTP requests and Pandas for data manipulation, to create comprehensive web scraping workflows.

However, it's important to note that web scraping should be done responsibly and in accordance with the terms of service and legal requirements of the websites you're scraping. Overly aggressive or unauthorized scraping can lead to legal issues and may impact the target website's performance. Always respect website policies and consider using web scraping for ethical and legitimate purposes.

This project aims at scraping the necessary data from the IMDB Top 250 movies list and Ambition box websites.

The following procedures can be followed as shown in the jupyter notebook in the repository:

import the necessary libraries

from bs4 import BeautifulSoup
import requests # Requests from the website for learning purpose and not for hacking
import os, sys
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
import statsmodels.api as sm
import scipy.stats as stats
from datetime import datetime
import warnings
warnings.filterwarnings('ignore')
%matplotlib inline
sns.set()
pd.set_option('display.max_rows',None)
pd.set_option('display.max_columns',None)
sns.set_style('whitegrid')

Loading the url and header to request access from the site

Using BeautifulSoup to extract the HTML data

Taking the titles in a list format

Please note: To extract the desired items, hover on to the data to be extracted and right click on top of it and tap the inspect tab, following which it leads to the html page which provides the
class and the tag selector and then add the same as shown in the jupyter notebook to extract all of the data of the same type.

Adding the same into a dataframe

Extracting details of year released, duration and ratings given

Filtering the data appropriately to obtain the required data in tabular format


## Ambition Box website

Extract the data required in the form of lists and then putting them into a tabular format

Filter the columns accordingly so as to obtain the data in appropriate columns and then the data is ready for further analysis.


The jupyter notebook provides end to end steps and instructions for basic web scraping for the above two websites.
