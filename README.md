# British Airways Customer Review Analysis
## Objective
Analyze customer reviews to identify key drivers of passenger satisfaction and areas for improvement.
## Key Insights
*	Passenger Concerns: Frequent mentions of seating arrangements, class types, food quality, delays, and service management.
###	Prerequisites
The tool requires the following Python libraries:
*	pandas: Data manipulation and analysis (1.1.0 or greater).
*	numpy: Numerical computing (1.19.0 or greater).
*	matplotlib: Visualization (3.3.0 or greater).
*	seaborn: Statistical data visualization (0.11.0 or greater).
*	nltk: Natural Language Toolkit for text processing (3.5 or greater). 
*	nltk.corpus: Provides access to stopword datasets.
*	nltk.tokenize: Tokenization of text.
*	nltk.stem: Lemmatization for stemming words to their base form.
*	wordcloud: Generates word clouds for text visualization (1.8.0 or greater).
*	BeautifulSoup (from bs4): HTML and XML parsing for web scraping (4.9.0 or greater).
*	requests: HTTP library for making web requests (2.25.0 or greater).
*	datetime: Handles date and time objects (built-in with Python 3.x).
*	time: Provides time-related functions (built-in with Python 3.x).
*	string: Contains string constants and functions (built-in with Python 3.x).
*	re: Regular expression operations (built-in with Python 3.x).
*	IPython.display: For interactive widgets and display in Jupyter Notebooks.

### Additional Notes:
*	nltk requires downloading specific datasets (e.g., stopwords, WordNet) using nltk.download().
*	BeautifulSoup is used for web scraping, and requests provides the interface to fetch web pages.
*	Visualization is supported by matplotlib, seaborn, and wordcloud.
  
# Understanding The Data

[import requests.docx](https://github.com/user-attachments/files/18136705/import.requests.docx)

This script is a basic web scraping setup that retrieves and prints the raw HTML of the specified webpage. It’s the first step in processing the page, which could involve further parsing or analysis using libraries like BeautifulSoup

[Load the dataset.docx](https://github.com/user-attachments/files/18136779/Load.the.dataset.docx)

The script processes a dataset of reviews, performing text cleaning and saving the cleaned data for further analysis. Here's a brief explanation:
1.	Load Dataset: The dataset (BA_reviews.csv) is loaded into a DataFrame with two columns: Review and Date.
2.	Text Cleaning Function:
*	Removes unwanted parts of the text ('Not Verified |').
*	Converts text to lowercase for uniformity.
*	Strips punctuation using str.translate.
*	Tokenizes text into words using word_tokenize.
*	Removes common stopwords (like "the", "and") using the stopwords list from NLTK.
*	Applies lemmatization to convert words to their base form using WordNetLemmatizer.
3.	Apply Cleaning: The clean_text function is applied to each review in the Review column, creating a new column cleaned_review.
4.	Drop Original Column: The original Review column is dropped as the cleaned version replaces it.
5.	Save Cleaned Data: The cleaned data, including the cleaned_review and Date columns, is displayed and optionally saved to a new CSV file (cleaned_reviews.csv) for further use.
 	
## Purpose
This script ensures the review text is standardized and simplified for text analysis tasks like sentiment analysis or NLP modeling.

[Preprocessing Reviews.docx](https://github.com/user-attachments/files/18136827/Preprocessing.Reviews.docx)

[sentiment and change over time.docx](https://github.com/user-attachments/files/18136899/sentiment.and.change.over.time.docx)




![image](https://github.com/user-attachments/assets/38b7db62-afa0-4a7e-b345-44c596d65a1d)![Sentimental Analysis](https://github.com/user-attachments/assets/08309209-8e3d-474f-8518-becde166b948)

![Changes over time](https://github.com/user-attachments/assets/7581c62b-d94e-4949-9ee8-f360f1cf24f9)


[Extracting Keywords from Negative Reviews.docx](https://github.com/user-attachments/files/18136974/Extracting.Keywords.from.Negative.Reviews.docx)


![Extracting Keywords](https://github.com/user-attachments/assets/51005c33-619f-4a8d-ab18-7942d2f1f80e)


[Quantitative analysis.docx](https://github.com/user-attachments/files/18136998/Quantitative.analysis.docx)


![QA](https://github.com/user-attachments/assets/af08e410-582d-4139-becd-0713904c436e)

### change over time Graph
This graph shows the trend of reviews over time, where the x-axis represents the years (from 2012 to 2024), and the y-axis represents the number of reviews for each year.
Key Observations:
1.	Increase in Reviews:
*	The number of reviews started very low in 2012 but rapidly increased to a peak around 2014-2015, where the number of reviews exceeded 700.
2.	Decline After the Peak:
*	After 2015, the number of reviews started to decline steadily, with some small fluctuations, until it hit its lowest point around 2020.
3.	Slight Recovery and Drop:
*	After 2020, there was a slight recovery in review numbers, peaking again in 2022, but then it dropped significantly by 2024.
  
# Inteerpretation:
*	The peak in reviews might reflect increased customer interaction or significant events during that period.
*	The sharp decline in later years could indicate less engagement or fewer issues prompting feedback.
*	Recovery in 2022 suggests renewed customer activity, which again tapered off in 2024.
This visualization helps to understand customer engagement patterns and track how interactions with reviews have changed over time.

