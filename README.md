# Sentiment_Prediction

Project Title: The Positive, the Negative, and Everything In Between: Sentiment Prediction in Movie Reviews

Project Description: We aim to classify the sentiment of movie reviews using 5 categorical labels: very negative, negative, neutral, positive, and very positive. As avid cinema enthusiasts, we are drawn to this project idea, as it has real-world applications in the natural language processing field.  

Database: We have chosen to use the sst5 database— which stands for the Stanford Sentiment Treebank. Composed of fine-grain labels detailing the positive/negative sentiments of movie reviews, the dataset includes 215,154 phrases and 11,855 sentences [1]. The training subset of this data is made up of 8,544 sentences, whereas the test includes 2,210 and the validation has 1,101.

Pre-processing: In order to assign each unique word with a numerical identifier, we performed tokenization across our training, test, and validation data. We also removed a select combination of stop-words in an effort to improve the eventual accuracy of our model. 

Model: To train our classifier, we will leverage a BERT-based deep learning model.

Works Cited:

1. [Recursive Deep Models for Semantic Compositionality Over a Sentiment Treebank](https://aclanthology.org/D13-1170) (Socher et al., EMNLP 2013)

