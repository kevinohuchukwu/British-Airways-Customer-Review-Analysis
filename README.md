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
# url = "https://www.airlinequality.com/airline-reviews/british-airways"


## Recommendations 
* Enhance meal quality and maintain seating comfort standards across all classes.
* Regularly review passenger feedback to address concerns proactively.
* Minimize delays through operational efficiency and improve transparency by providing timely updates.

# Predictive Model for Understanding Buying Behavior
## Objective
Develop predictive models to identify factors influencing booking behavior and optimize revenue potential.
Key Insights
* Top Predictors: Purchase lead time, route, booking origin, flight hour, length of stay, and flight duration.
## Model Performance: 
*  Gradient Boosting performed better on ROC-AUC (0.7871) but struggled with recall for completed bookings.
*  Random Forest effectively predicted non-booking events but also showed poor recall for completed bookings.
  ## Challenges 
* Class imbalance biased predictions toward non-bookings (Class 0), reducing accuracy for completed bookings (Class 1).

# Recommendations: 
*  Target high-value routes and origins with promotions.
*  Implement early-bird discounts to encourage earlier bookings.
*  Retarget at-risk customers with personalized offers.
*  Address model imbalance with oversampling, class-weight adjustments, or ensemble techniques to improve recall.
