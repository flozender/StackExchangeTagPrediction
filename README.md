# Stack Exchange Question Tag Assignment
#### SOEN 471/SOEN 6111 - Big Data

## Project Definition
Thousands of questions are asked on Stack Exchange everyday, which makes navigating through the vast collection of questions difficult. Question tagging is a feature that helps categorize a question broadly, in an attempt of grouping questions of similar topics or fields together. The goal of our project is to appropriately predict these tags for questions that were asked by users of [Stack Exchange](https://stackexchange.com).

### Dataset and Characteristics
[Our dataset](https://www.kaggle.com/c/facebook-recruiting-iii-keyword-extraction/) contains four attributes, namely ID, Title, Body, and Tags. The dataset will be divided into testing and training sets. Each row in the dataset contains the title and body text for a question, along with a set of space-separated tags attached to the question. As tags are user-defined, there isn't a set of predefined tags. From our initial analysis, we found that in the first 50,000 questions, we had a set of 13,893 different tags. To apply our approach of using one Decision Tree Classifier (DTC) per tag, we will analyze all the tags and select the top 500 tags to make one DTC each. 

### Research Questions

### Machine Learning Models and Algorithms
