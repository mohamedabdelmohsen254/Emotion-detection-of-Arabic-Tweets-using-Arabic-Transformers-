# Emotion-detection-of-Arabic-Tweets-using-Arabic-Transformers-
This study aims to Compare state-of-the-art Arabic transformer models (ArBERT, MarBERT, AraBERT, AraBERT-Twitter, Qarib) in a large Arabic dataset and improve their results using different prepossessing techniques.

## PROBLEM STATEMENT
Social media platforms have become an essential means for communicating feelings to the entire world due to rapid expansion in the Internet era and Nowadays people can express their feelings and thoughts using pictures, videos, audio, or textual content and this led to a massive amount of unstructured data generated from this Social media platforms and The question is **what if we can use this data to detect the emotions and feelings of the users?**

There is a growing interest in using emotion analysis on the Arabic text to understand public reactions and this could be useful in many fields such as monitoring people’s mental health, especially after crises and pandemics such as covid-19 where Surveys by such organizations as YouGov show that, during the pandemic, workers were more stressed than ever.

The Arabic language is now facing many problems due to the increase in verb conjugations, the formation, and the presence of more than one word that leads to the same meaning, and many other problems that we should put into considerations when we work in Arabic text

The purpose of this study is to Compare state-of-the-art Arabic transformer models in Nile University Dataset, which  comprised of 10,065 tweets and categorized into 8 emotions (sadness, anger, fear, sympathy, joy, surprise, love, and none) and our aim is to improve the models' results using Different combinations of prepossessing techniques so  that, we can use them in emotion detection

## Methodology
### Dataset
The dataset was collected by a research group at Nile University (NU). It is a balanced dataset consists of 10,065 Arabic tweets mostly using Egyptian dialect, and was manually annotated using eight emotions (sadness, anger, joy, surprise, love, sympathy, fear and none). It was collected using the” Olympics” hashtags from Egypt in the period between Jul 2016 and Aug 2016. The dataset was split into 80% for training and 20% for testing.

### Preprocessing techniques
Data pre-processing is important to minimize the noise and get a better classification accuracy and we applied a lot of techniques in preprocessing the Arabic text such as removing stop words, non-Arabic letters and spaces, Diacritics, Punctuation, Links, mentions, retweet indicators and suffixes and prefixes also, we reduced the Arabic words to their roots using different stemmers and we handled emojis

### Experimental design
We have done 3 experiments on this dataset where each of them started by using the same pre-processing techniques in with some small changes, in the first experiment we removed the emojis and emoticons from the dataset and we used this data in Arabic Transformer models to measure the performance and in the second experiment we replaced emojis and emoticons with an equivalent Arabic emotion to see that if this step will give us better accuracy, and in the last experiment we replaced each emoticon with it’s equivalent emoji and we kept the emojis in the dataset as it is and we passed this data in AraBERT-Twitter model as this model have had emojis added to their vocabulary and the

###Performance metrics:
Accuracy, precision, recall, and F-score were used. For each classifier, the error metrics were calculated for each individual label (joy, sadness, sympathy, anger, fear, surprise, love, none). The final error metrics were calculated as the average of all the metrics for all the labels.

## Results
### Arabic Transformer models
We used AraBERT-Base, AraBERT-Twitter, MarBERT, ArBERT and Qarib and best results were when we used MarBERT model in experiment 2 as expected we got 77% accuracy, 76.8% Precision, 76.2% Recall and 76.2% F- score and these results are the best among all the previous work on this dataset It was expected that the results from experiment 2 will be the best one because of the mapping of the emojis we did and also, MarBERT according to it’s Arciheture we expected that it will have the best performance and In case of AraBERT-Twitter it performs better in experiment 1 than experiment 3 where we kept the emojis
**More details will be in the research paper uploaded**

[Emotion detection of Arabic Tweets using Arabic Transformers.pdf](https://github.com/mohamedabdelmohsen254/Emotion-detection-of-Arabic-Tweets-using-Arabic-Transformers-/files/9447747/Emotion.detection.of.Arabic.Tweets.using.Arabic.Transformers.pdf)
