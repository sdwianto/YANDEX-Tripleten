## Develop model to automatically detect negative reviews
#### <i>Sprint focus: Machine Learning for Text, bag-of-word (BoW), N-Gram, TF-IDF, Tokenization, Lemmatization, Corpus, Regular Expression, Text Analysis, Sentiment Analysis, Word Embedding, Word2vec, BERT </i>

Summary: 
Film Junky Union, a new community for classic film enthusiasts, is developing a system to filter and categorize film reviews. The main mission is to train a model to automatically detect negative reviews. The dataset used for this task is IMDb film reviews with polarity labeling, and the goal is to create a model that can classify reviews as either positive or negative with an F1 score of at least 0.85.

Conclusion: 
Several models were evaluated for the task of classifying film reviews as positive or negative. The results for each model are as follows:
1.	Linear Regression with NLTK and TF-IDF:
-	Maximum F1 score on train set: 0.79
-	Maximum F1 score on test set: 0.77
-	Maximum ROC-AUC score on train set: 0.85
-	Maximum ROC-AUC score on test set: 0.84
-	Maximum recall score on train set: 0.85
-	Maximum recall score on test set: 0.84
2.	Linear Regression with spaCy and TF-IDF:
-	Maximum F1 score on train set: 0.8
-	Maximum F1 score on test set: 0.77
-	Maximum ROC-AUC score on train set: 0.85
-	Maximum ROC-AUC score on test set: 0.84
-	Maximum recall score on train set: 0.85
-	Maximum recall score on test set: 0.83
3.	LGBM Classifier with spaCy and TF-IDF:
-	Maximum F1 score on train set: 0.86
-	Maximum F1 score on test set: 0.79
-	Maximum ROC-AUC score on train set: 0.87
-	Maximum ROC-AUC score on test set: 0.81
-	Maximum recall score on train set: 0.86
-	Maximum recall score on test set: 0.79
  
The third model (spaCy, TF-IDF, and LGBM Classifier) outperforms the second and third models, providing higher prediction values for the reviews.
