# SMS Spam Detection Using Machine Learning

## Project Overview

This project uses Natural Language Processing (NLP) and machine learning to classify SMS messages as spam or legitimate (ham). It compares two classification algorithms and uses the better-performing model to predict new messages.

## Objective

To build a machine learning model that identifies unwanted or fraudulent SMS messages and distinguishes them from legitimate messages.

## Dataset

* **Source:** SMS Spam Collection dataset hosted on GitHub
* **Original records:** 5,572 messages
* **Duplicate rows removed:** 403
* **Records after removing duplicates:** 5,169
* **Target labels:** Spam and Ham

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Natural Language Processing (NLP)
* TF-IDF Vectorization
* Pickle

## Machine Learning Models

1. **Multinomial Naive Bayes**
2. **Logistic Regression**

## Project Workflow

1. Loaded and explored the SMS dataset.
2. Checked missing values and duplicate records.
3. Removed duplicate messages.
4. Cleaned the text by converting it to lowercase and removing numbers, punctuation, and extra spaces.
5. Converted text into numerical features using TF-IDF vectorization.
6. Split the dataset into training and testing sets.
7. Trained and evaluated both classification models.
8. Compared model performance using accuracy, precision, recall, and F1-score.
9. Saved the selected model and TF-IDF vectorizer.
10. Tested the saved model on new SMS messages.

## Model Performance

| Metric    | Multinomial Naive Bayes | Logistic Regression |
| --------- | ----------------------: | ------------------: |
| Accuracy  |                  97.20% |              94.68% |
| Precision |                 100.00% |              98.72% |
| Recall    |                  77.86% |              58.78% |
| F1-score  |                  87.55% |              73.68% |

## Selected Model

Multinomial Naive Bayes was selected because it achieved better overall performance on the test dataset, with 97.20% accuracy and an 87.55% F1-score.

Although its precision was 100% on the test set, its recall was 77.86%, meaning that some spam messages were not detected.

## Sample Prediction

**Input:** Congratulations! You have won a free prize. Call now!

**Prediction:** Spam

The saved model was successfully loaded and tested.

## Project Files

* **Jupyter Notebook:** Data exploration, text preprocessing, model training, evaluation, and predictions.
* **sms_spam_model.pkl:** Saved Multinomial Naive Bayes model.
* **tfidf_vectorizer.pkl:** Saved TF-IDF vectorizer.

## How to Run

1. Clone or download this repository.
2. Install the required Python libraries.
3. Open the Jupyter Notebook and run the cells in order.

Required libraries can be installed using:

`pip install pandas numpy matplotlib seaborn scikit-learn`

## Conclusion

This project demonstrates how NLP and machine learning can be used to classify SMS messages. Multinomial Naive Bayes outperformed Logistic Regression in the evaluation, and the saved model successfully classified a sample spam message.

**Note:** Model performance is based on the selected train-test split and may vary on unseen messages.

## Internship

Oasis Infobyte — Data Science Internship
