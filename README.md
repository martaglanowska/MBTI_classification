# Personality Type Classification Based on Internet Posts

This work is a set of experiments in the field of text classification. The project uses a number of traditional machine learning methods and neural networks. The technique for creating a numerical representation of text was selected depending on the characteristics of the model.

The project served as the practical part of my master's thesis.

## Abstract
The modern world emphasizes the importance of constant personal development and 
encourages conscious exploration of one's interior and the patterns operating within it. This 
is manifested, among others, in the business sphere, where soft skills are increasingly talked 
about and financial resources are allocated to the development of employees' natural 
abilities. One of the tools well embedded in this reality are personality tests, which, however, 
take a certain amount of time to conduct. A good alternative could be an automatic 
personality recognition system based on other types of data. The presented work examines 
the possibilities of using machine learning and artificial intelligence methods in the problem 
of classifying sixteen personality types of the MBTI model. The basis for modeling was 
a database of actual entries posted on the Internet. They turned out to be a valuable source 
of information about the authors' personality types. During the research, experiments were 
carried out using four traditional machine learning algorithms and four neural network 
architectures built using modern text processing blocks. The evaluation of the value of the 
accuracy measure and the 𝐹1 index of the proposed structures clearly distinguished the 
XGBoost model as the most effective solution, with results competitive to other strategies 
available in the literature. The result of the study confirms the usefulness of machine learning 
methods in the psychological field. It highlights the potential of tools based on trained models 
to support professionals working with personality tests in their everyday challenges.

## Dataset
Authentic text samples come from Kaggle platform: https://www.kaggle.com/datasets/datasnaek/mbti-type.

## Methods
*Text preprocessing:* including tokenization, stopwords removal, marking characteristic elements, 80:20 stratified split.

*Traditional approach:* 
 * TF-IDF representation (unigrams, bigrams, unigrams & bigrams)
 * multinomial logistic regression, linear SVM classifiers, multinomial Naive Bayes classifier, extreme gradient boosting (XGBoost)

*Neural networks:* 
 * embedding in 64 dimensional space
 * RNN with GRU Cell (with optimization attempt), neural network with Attention mechanism

*BERT:* 
 * dedicated preprocessing model
 * BERT fine-tuning
