# phase4_group_5

# Apple_Google sentiment Analysis
### Project Overview
Group 5 aims to develop an ML model for sentiment analysis of tweets about Apple and Google products. Using advanced NLP techniques, 
the model will classify tweets as positive, negative, or neutral. Insights will empower stakeholders—Product Management, Marketing, Customer Experience,
 Business Intelligence, and Leadership Teams—to make data-driven decisions, improve marketing, enhance customer satisfaction, and drive 
 innovation.

 ## Business Understanding
 The dataset captures tweets about Apple and Google products or services to understand public sentiment. These insights help the brands assess 
 customer satisfaction, spot areas for improvement, track perceptions during events like SXSW, and refine strategies to boost customer 
 engagement and loyalty.

 __Problem Statement:__ Creating a reliable sentiment analysis model to accurately identify positive and negative customer sentiments about
  Apple and Google products on Twitter, with a special focus on better detecting negative feedback.

  ### Primary Objective

- Building a machine learning model to accurately classify the sentiment of tweets—positive, negative, or neutral—based on their content.

### Secondary Objectictives
- Compare Brand Sentiments: Analyze and report differences in consumer sentiment between Apple and Google.
- Enhance Negative Feedback Detection: Improve the ability to identify and capture negative sentiments effectively
- Support Stakeholder Decisions: Provide actionable insights for marketing, customer service, and leadership teams.

## Metrics of Success

- Accuracy: Achieve at least 70% accuracy, reflecting the model's overall reliability in correctly classifying sentiments across all categories
- Precision: Attain a precision of 65%, ensuring that when the model identifies tweets as positive or negative, the predictions are consistently accurate.
- Recall: Ensure the model catches as many actual negative tweets as possible, minimizing the chances of missing important negative feedback.
- F1 Score: The F1 score shows how well the model balances being accurate (precision) and not missing important feedback (recall). A higher 
score means the model is good at correctly identifying sentiments while catching as many relevant tweets as possible.
- Sentiment Class Balance: Make sure the model treats all sentiment types (positive, negative, and neutral) fairly. This means it shouldn't 
favor one type over others or perform much better on one while struggling with the rest.

## Data Understanding

The dataset, sourced from CrowdFlower via Data.World, contains 9,093 tweets carefully labeled by human raters with sentiment categories: 
positive, negative, or neutral. Collected in March, around the SXSW event, the tweets were filtered using specific hashtags and keywords.
The dataset includes the following three columns:
**tweet_text:** The actual text of the tweet, which provides insights into what users are saying about Apple and Google products.

**emotion_in_tweet_is_directed_at:** The specific product or brand mentioned (e.g., iPhone, iPad, Google).


**is_there_an_emotion_directed_at_a_brand_or_product:**  Indicates whether the tweet expresses positive, negative, no emotion, or is unclear 
about the sentiment toward a brand or product.


### Imported the relevant libraries 

Loaded the data and inspected it by viewing the columns the dimensionality the datatypes

### Data cleaning
- Checked for missing values Duplicates
- Handled the missing values and Duplicates

#### NLP Text Cleaning
We clean the text data by performing the following steps:

- Converts the text to lowercase to standardize it.
- Tokenizes the text using regex to split it into words.
- Removes stopwords and non-alphabetic words.
- Lemmatizes each word to reduce it to its base form.
- The cleaned text is stored in a new column, cleaned_tweet, for further analysis.


## Exploratory Data Analysis(EDA)
- **Top Mentions:** iPad, Google, Apple, and iPhone dominate tweets, highlighting their popularity and relevance.
- **Sentiment Distribution:** Most responses are neutral, followed by positive sentiment, with negative sentiment being the least frequent, reflecting overall neutrality with a tilt toward positivity.
- **iPad's Strength:** iPad leads in positive sentiment, indicating high user satisfaction and strong emotional connection.
- **Google's Neutral Sentiment:** Google dominates neutral sentiments, suggesting reliability and utility but less emotional engagement.
**Brand Emotional Trends:**
- **Apple:** High neutral and positive sentiment, showing broad user satisfaction.
- **Google:** Wider mix of emotions, with a focus on neutrality and positivity.
- **Other Brands:** Less emotional engagement overall.

#### Strategic Insights
Apple can capitalize on its positive emotional connection, while Google has an opportunity to foster greater emotional engagement.

### Modeling
Tried several models and support vector  machine (SVM) gave us better results than the rest.
Predicting 72% accurately most times.
This is even before hyperparametor tuning 
### Recommendation
- Neutral Sentiment Toward Google: A notable share of neutral sentiment around Google products highlights an opportunity to generate excitement 
through more dynamic and engaging marketing efforts.
- Addressing Recurring Issues for Google: Tweets expressing neutral or negative sentiment about Google often point to usability challenges. 
Implement targeted support initiatives or comprehensive FAQs to address these issues proactively and reduce potential dissatisfaction.
- Apple's Strengths and Opportunities: Although Apple enjoys strong positive sentiment, it's important to track any emerging concerns to ensure
 the brand maintains its dominant market position.

### Conclusion
Our analysis reveals key opportunities: Apple can strengthen its market leadership by leveraging positive sentiment and addressing emerging
 concerns, while Google can close sentiment gaps, particularly around neutrality and usability, through targeted marketing and support. 
 The SVM model’s strong performance makes it the best choice for immediate implementation.

### Next steps
Deploy the model with a comprehensive monitoring system to track key metrics, including accuracy and recall for the Negative class, 
ensuring reliable performance over time. 







