# Enhanced Customer Insight Through Sentiment Analysis of Online Reviews

## Project Overview

This project implements a hybrid sentiment analysis model that combines the lexicon-based VADER tool with machine learning techniques, specifically logistic regression, to enhance the accuracy and efficiency of sentiment analysis. The analysis is performed on a dataset of Amazon Alexa product reviews.

 ## Datasets

 The dataset contains 3,150 reviews of Amazon Alexa products, each with the following attributes:

	•	rating: Product rating (1 to 5 stars).
	•	date: Date of the review.
	•	variation: Product variation (e.g., “Charcoal Fabric”).
	•	verified_reviews: The text of the review.
	•	feedback: A binary label indicating whether the review is positive (1) or negative (0).

 ## Methodology

#### Data Preprocessing:
	•	The text is cleaned by converting it to lowercase and removing non-alphanumeric characters.
	•	Stopwords are removed, and the text is lemmatized using the NLTK library to focus on the most meaningful words.
#### Sentiment Analysis:
	•	VADER is used to compute sentiment scores for each review.
#### Feature Extraction:
	•	TF-IDF vectorization converts the cleaned text data into numerical features that emphasize unique words in each review.
#### Model Development:
	•	A logistic regression model is trained using both VADER sentiment scores and TF-IDF features.
	•	The dataset is split into training and testing sets to evaluate model performance.
#### Model Evaluation:
	•	The model achieved a 93% accuracy, demonstrating the effectiveness of combining VADER with machine learning techniques.

 ## Results
 
 The hybrid model significantly improves the accuracy of sentiment analysis, effectively capturing nuanced sentiments that may be overlooked by either VADER or logistic regression alone.

 ## Conclusion

 This project showcases the potential of a hybrid sentiment analysis model to provide more accurate insights into customer feedback, which is critical for improving product offerings and customer service.
