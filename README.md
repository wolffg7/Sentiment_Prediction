# Sentiment_Prediction: Abstract / ReadMe

Team Members: Wolff Gilligan and Ethan McFarlin, AIT Budapest Spring 2023

Project Title: The Positive, the Negative, and Everything In Between— Sentiment Prediction in Movie Reviews Using Deep Learning

Full Documentation: [click here](https://docs.google.com/document/d/1JGz4GjbxrzFUUXuc9B2sKRmqLz6bmyH9sU8HfGTQ8SM/edit?usp=sharing)

Presentation Link: [click here](https://docs.google.com/presentation/d/1supNDNH-lGQWGH6QKr9jTHkWpu9eR1Y9/edit?usp=sharing&ouid=117979881791114394248&rtpof=true&sd=true)

Project Description: We aim to classify the sentiment of movie reviews using 5 categorical labels: very negative, negative, neutral, positive, and very positive. As avid cinema enthusiasts, we are drawn to this project idea, as it has real-world applications in the natural language processing field.  

Database: We have chosen to use the sst5 database— which stands for the Stanford Sentiment Treebank. Composed of fine-grain labels detailing the positive/negative sentiments of movie reviews, the dataset includes 215,154 phrases and 11,855 sentences [1]. The training subset of this data is made up of 8,544 sentences, whereas the test includes 2,210 and the validation has 1,101.

Pre-processing: We began this stage by removing a select combination of stop-words from the input sentences. In order to assign each word with a unique numerical identifier, we performed a form of tokenization adapted for BERT across our training and test data. 

Model: Our sentiment prediction leverages a pre-trained BERT deep learning model [2]. The attention mask and input ID's are passed into BERT. Then, the model is fitted to the data and evaluated for performance. We further train the model using custom, Chat-GPT-generated labels through the OpenAI API.

Works Cited:

1. [Recursive Deep Models for Semantic Compositionality Over a Sentiment Treebank](https://aclanthology.org/D13-1170) (Socher et al., EMNLP 2013)
2. [BERT language model](https://www.techtarget.com/searchenterpriseai/definition/BERT-language-model) (Ben Lutkevich, TechTarget 2020)

Database Link:

1. https://huggingface.co/datasets/SetFit/sst5
