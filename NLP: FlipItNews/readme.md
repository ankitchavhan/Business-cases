## Context:

- The Gurugram-based company ‘FlipItNews’ aims to revolutionize the way Indians perceive finance, business, and capital market investment, by giving it a boost through artificial intelligence (AI) and machine learning (ML). They’re on a mission to reinvent financial literacy for Indians, where financial awareness is driven by smart information discovery and engagement with peers. Through their smart content discovery and contextual engagement, the company is simplifying business, finance, and investment for millennials and first-time investors


## Objective:

- The goal of this project is to use a bunch of news articles extracted from the companies’ internal database and categorize them into several categories like politics, technology, sports, business and entertainment based on their content. Use natural language processing and create & compare at least three different models.

## Attribute Information:
  - Article
  - Category

## What does ‘good’ look like?
- Installing & Importing all the required libraries and Loading the dataset.
- Conduct a preliminary analysis to understand the structure of the dataset and the distribution of news articles in each category.
- Create a user defined function to process the textual data (news articles).
  - Remove non-letters
  - Remove Stopwords
  - Word Tokenize the text
  - Perform Lemmatization
- Display how a single news article looks like before and after the processing.
- Encode the target variable (category) using Label/Ordinal encoder.
- Create an option for the user to choose between Bag of Words and TF-IDF techniques for vectorizing the data.
- Perform train-test split and train a Naive Bayes classifier model using the simple/classical approach.
- Evaluate the model’s performance and plot the Confusion Matrix as well as Classification Report.
- Functionalize the code and train & evaluate three more classifier models (Decision Tree, Nearest Neighbors, Random Forest).
- Observe and comment on the performances of all the models used.


## Questionnaire:
1. How many news articles are present in the dataset that we have?
2. Most of the news articles are from _____ category.
3. Only ___ no. of articles belong to the ‘Technology’ category.
4. What are Stop Words and why should they be removed from the text data?
5. Explain the difference between Stemming and Lemmatization.
6. Which of the techniques Bag of Words or TF-IDF is considered to be more efficient than the other?
7. What’s the shape of train & test data sets after performing a 75:25 split.
8. Which of the following is found to be the best performing model..
  - Random Forest
  - Nearest Neighbors
  - Naive Bayes
9. According to this particular use case, both precision and recall are equally important. (T/F)
