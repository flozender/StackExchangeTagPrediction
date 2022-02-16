# Stack Exchange Question Tag Assignment

#### SOEN 471/SOEN 6111 - Big Data - Team 17

## Project Definition

Thousands of questions are asked on Stack Exchange everyday, which makes navigating through the vast collection of questions difficult. Question tagging is a feature that helps categorize a question broadly, in an attempt of grouping questions of similar topics or fields together. The goal of our project is to appropriately predict these tags for questions that were asked by users of [Stack Exchange](https://stackexchange.com).

### Dataset and Characteristics

[Our dataset](https://www.kaggle.com/c/facebook-recruiting-iii-keyword-extraction/) contains four attributes, namely ID, Title, Body, and Tags. The dataset will be divided into testing and training sets. Each row in the dataset contains the title and body text for a question, along with a set of space-separated tags attached to the question. As tags are user-defined, there isn't a set of predefined tags. From our initial analysis, we found that in the first 50,000 questions, we had a set of 13,893 different tags. To apply our approach of using one Decision Tree Classifier (DTC) per tag, we will analyze all the tags and select the top 500 tags to make one DTC each. The dataset contains a total of 6,034,195 questions with tags attached.

### Research Questions

One of the most pertinent questions that we will have to answer will be related to the approach we use in trying to make the predictions. Will a model designed around producing predictions based on the frequency of the appearance of certain words be sufficient, or will the extraction of some type of 'meaning' from the combination of words using NLP technology be necessary in developing predictions that are adequately useful?
This will be answered by comparing models developed using both methods. Which model is more effective? Which model is more difficult to develop and train? Are the tradeoffs worth it? All of these questions will need to be answered before deciding on the model to use for our project.
Another important question that is related to the feasibility of our project as a whole is how often people use tags in their stack exchange posts. This will directly affect the possible size of our training sets, and thus the plausibility of developing an effective model.

### Machine Learning Models and Algorithms

We will be using two main pre-processing techniques - TFIDF and Word Embeddings to build our input features, which will then be used with supervised classification algorithms such as Decision Trees. Another type of algorithm we hope to implement is Long-Short Term Memory (LSTM) neural networks.
