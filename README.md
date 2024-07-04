# HOPE at IberLEF 2024
# Team Name : MUCS
# Title : Hope on the Horizon: Experiments with Learning Models for Hope Speech Detection in Spanish and English

Hope is the expectation or belief that results in positive outcomes despite challenges or adversity and "hope speech" refers to text
aimed at inspiring hope, motivation, or positivity. Individuals who are experiencing challenges may be inspired from hope speech
as it instills optimism, encouragement, and positivity. On social media platforms, hope speech contributes to fostering a positive
and supportive community, offering comfort, motivation, and solidarity to online users. 
A healthy social media echo system can be maintained by identifying and amplifying the hope speech content In this direction, “HOPE at IberLEF 2024” shared task organized at IberLEF 2024, invites the research community to address the challenges of detecting hope speech in Spanish and English languages. The shared task consists of two tasks: Task 1: Hope for Equality, Diversity and Inclusion (EDI) - a binary classification problem in Spanish language where the train set consists of text in LGTBI domain and test set in unknown domains, and Task 2: Hope as Expectations (HE) consisting of two subtasks: 2.a) Binary Hope Speech detection and 2.b) Multiclass Hope Speech detection, both in Spanish and English languages. To explore the strategies for detecting hope speech in Spanish and English on social media platforms, in this paper, we - team MUCS, describe the models submitted to these tasks. Various Machine Learning (ML) models and Transfer Learning (TL) techniques are proposed to classify the given Spanish and English text into : i) one of the two categories - ’nhs’/’Not Hope’ or ’hs’/’Hope’ in case of binary classification and ii) one of the four categories - ’Not Hope’, ’Generalized hope’, ’unrealistic hope’, or ’realistic hope’ in case of multiclass classification. While Term Frequency-Inverse Document Frequency (TF-IDF) of word n-grams in the range (1,3), multilingual embeddings, and aligned word vectors, are used as features to train the different ML models individually, Bidirectional Encoder Representations from Transformers (BERT) variants are fine-tuned in TL models, to detect hope speech in Spanish and English.

The best results obtained by our proposed models are: 10th rank with macro F1 score 0.59 in Task 1 HopeEDI, 5th and 9th ranks for
Spanish and English respectively with macro F1 scores 0.82 and 0.82 in subtask 2.a) Binary hope speech detection, and 4th and 8th ranks
for Spanish and English respectively with macro F1 scores 0.64 and 0.56 in subtask 2.b) Multiclass hope speech detection.

The methodology includes balancing the imbalanced data provided by the organizers of the shared task followed by constructing ML and TL models. Data imbalance occurs when there is a large variation in the number of instances within the given classes. In such cases, the learning models demonstrate a bias for the majority class while performing poor for the minority class. This bias could be reduced to
some extent by balancing the dataset either by increasing the minority class samples or decreasing the majority class. 

**Two distinct techniques are used to balance the dataset, they are: Random oversampling, Natural Language Processing Augmentation (NLPAug)**. 

# Models used are:
# Task 1: EDI  
* Various ML models
* TL model
* Hope_Probfuse
# Task 2: Spanish Binary Hope Speech detection 
* TL models
* Hope_probfuse
# Task 2: English Binary Hope Speech detection
  * ML models
  * ML - RF model with logloss function
  * TL_BERT
# Task 2: Spanish Multiclass Hope Speech detection
* ML models
* TL models
# Task 2: English Multiclass Hope Speech detection
* ML models
* Hope_probfuse
# Task 2: Multilingual models
* TL_Ensemble model
* TL_mBERT
* ML models

-- The code of the respective models utlized are uploaded in this repository. 
