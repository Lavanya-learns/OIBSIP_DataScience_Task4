# SMS Spam Detection Using Machine Learning

## Project Overview

This project uses Natural Language Processing (NLP) and machine learning to classify SMS messages as spam or legitimate (ham).

## Dataset

* Source: SMS Spam Collection dataset hosted on GitHub
* Original messages: 5,572
* Duplicate rows removed: 403
* Messages after cleaning: 5,169

## Technologies Used

* Python
* Pandas and NumPy
* Matplotlib and Seaborn
* Scikit-learn
* TF-IDF Vectorization
* Multinomial Naive Bayes
* Logistic Regression

## Methodology

1. Loaded and explored the dataset.
2. Checked missing values and duplicate messages.
3. Removed duplicate rows.
4. Preprocessed SMS text by converting it to lowercase and removing numbers and punctuation.
5. Converted text into numerical features using TF-IDF.
6. Split the data into training and testing sets.
7. Trained Multinomial Naive Bayes and Logistic Regression models.
8. Evaluated performance using accuracy, precision, recall, F1-score, and confusion matrices.
9. Saved the selected model and TF-IDF vectorizer.
10. Tested the saved model on new SMS messages.

## Model Results

| Metric    | Multinomial Naive Bayes | Logistic Regression |
| --------- | ----------------------: | ------------------: |
| Accuracy  |                  97.20% |              94.68% |
| Precision |                 100.00% |              98.72% |
| Recall    |                  77.86% |              58.78% |
| F1-score  |                  87.55% |              73.68% |

## Conclusion

Multinomial Naive Bayes performed better than Logistic Regression on the test set, achieving 97.20% accuracy and an 87.55% F1-score. The saved model successfully classified a sample promotional message as spam.

The recall score indicates that some spam messages were missed, so further improvements could focus on detecting more spam while maintaining high precision.

## Project Files

* Jupyter Notebook: data exploration, preprocessing, training, and evaluation
* `sms_spam_model.pkl`: saved Multinomial Naive Bayes model
* `tfidf_vectorizer.pkl`: saved TF-IDF vectorizer
