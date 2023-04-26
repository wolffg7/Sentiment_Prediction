# Sentiment_Prediction: Abstract / ReadMe

Team Members: Wolff Gilligan and Ethan McFarlin, AIT Budapest Spring 2023

Project Title: The Positive, the Negative, and Everything In Between— Sentiment Prediction in Movie Reviews Using Deep Learning

Project Description: We aim to classify the sentiment of movie reviews using 5 categorical labels: very negative, negative, neutral, positive, and very positive. As avid cinema enthusiasts, we are drawn to this project idea, as it has real-world applications in the natural language processing field.  

Database: We have chosen to use the sst5 database— which stands for the Stanford Sentiment Treebank. Composed of fine-grain labels detailing the positive/negative sentiments of movie reviews, the dataset includes 215,154 phrases and 11,855 sentences [1]. The training subset of this data is made up of 8,544 sentences, whereas the test includes 2,210 and the validation has 1,101.

Pre-processing: We began this stage by removing a select combination of stop-words from the input sentences. In order to assign each word with a unique numerical identifier, we performed a form of tokenization adapted for BERT across our training, test, and validation data. We also structured our tokenized data such that sentences are bound to their corresponding sentiments. Then, to ensure that each index is formatted with a uniform number of words, we calculated the maximum sentence length and distributed padding across the dataset. In the process of doing so, we built out an attention mask for the BERT model, which helps it to distinguish between padded and non-padded sequences. Equipped with padded sequences and an attention mask, both data structures were converted to a NumPy array in preparation for the proceeding stage, defining the model.

Model: To train our classifier, we will leverage a BERT-based deep learning model. Looking ahead to the next steps, we plan to officially bring our deep learning model to fruition, fine tune its parameters, assess its performance using our test set, and lastly, introduce new test data which uses ChatGTP labels.

Works Cited:

1. [Recursive Deep Models for Semantic Compositionality Over a Sentiment Treebank](https://aclanthology.org/D13-1170) (Socher et al., EMNLP 2013)

Database Link:

1. https://huggingface.co/datasets/SetFit/sst5
