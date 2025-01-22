Sentiment Analysis of Product Reviews

This repository contains a comprehensive analysis of product reviews, focusing on text preprocessing, sentiment analysis, and feature engineering. The aim is to extract meaningful insights to help businesses enhance their products and improve customer satisfaction.


Dataset Description

The dataset includes product reviews with the following fields:

categories: Categories associated with the product.

primaryCategories: Main product category.

reviewsdate: Date of the review.

reviewstext: Full review text provided by the customer.

reviewstitle: Title of the review.

sentiment: Manually labeled sentiment (Positive, Negative, Neutral).

Additional derived fields include:

review_year, review_month, review_day: Extracted from the review date.

Review_Length: Length of the review text.

cleaned_reviews: Preprocessed version of the review text.

word_count: Total number of words in the review.

sentiment_score: Numerical polarity score of the sentiment.

Workflow

1. Data Preprocessing

Converted reviews.date to datetime format.

Extracted year, month, and day for time-based analysis.

Cleaned text by:

Converting to lowercase.

Removing punctuation and stopwords.

Applying tokenization and lemmatization.

2. Sentiment Analysis

Used VADER and TextBlob for sentiment scoring.

Analyzed positive, negative, and neutral sentiments through word clouds and distribution plots.

Observed themes in customer feedback based on sentiment.

3. Feature Engineering

Added features like Review_Length, word_count, and sentiment_score.

Vectorized cleaned text using Tf-Idf for numerical representation.

Combined textual and numerical features for model-ready data.

4. Visualizations

Generated word clouds to identify common words for each sentiment.

Plotted review length distributions by sentiment category.

Created a feature correlation heatmap for numerical data.

Results and Insights

1. Sentiment Trends

Positive Reviews: Shorter and concise with terms like "great," "recommended," and "product."

Negative Reviews: Longer and descriptive, highlighting dissatisfaction (e.g., "disappointing," "expected").

Neutral Reviews: Mixed opinions with mentions of "value," "quality," and "money."

2. Key Observations

Positive reviews are generally brief and focused on straightforward praise.

Negative reviews tend to be more detailed, elaborating on specific issues.

Neutral reviews often balance details and brevity, reflecting moderate satisfaction.

3. Feature Relationships

Sentiment scores and review lengths correlate with the tone and quality of the review.

Word count provides insights into the level of detail customers provide in their feedback.

Suggestions for Improvement

Focus on Quality: Address issues commonly cited in negative feedback.

Encourage Detailed Feedback: Request more descriptive reviews from satisfied customers.

Enhance Neutral Feedback: Improve product features to shift neutral reviews toward positivity.

Marketing Campaigns: Leverage positive themes like "highly recommended" in promotions.

Dashboard Creation: Develop a dashboard to monitor sentiment trends and review themes.



Technologies Used

Libraries: pandas, numpy, matplotlib, seaborn, nltk, sklearn, wordcloud, TextBlob

NLP Tools: VADER, Tf-Idf vectorizer, WordNetLemmatizer

Visualization: Word clouds, sentiment distribution plots, correlation heatmaps



How to Use

Clone the repository:

git clone https://github.com/your-repo/sentiment-analysis.git

Install required libraries:

pip install -r requirements.txt

Run the analysis script:

python analysis.py

Review visualizations and insights from the generated outputs.
