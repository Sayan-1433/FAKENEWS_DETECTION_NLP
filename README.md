This repository contains code for a Fake News Detection System that analyzes tweets and classifies them as "Real" or "Fake" using Natural Language Processing (NLP) and Machine Learning models.

## Files:

* **`fake_news_detection.ipynb`**: This Jupyter Notebook contains the core logic for training and evaluating different machine learning models for fake news detection. It explores various vectorizers (CountVectorizer) and text preprocessing functions (NLTK, spaCy) with models like Logistic Regression and Naive Bayes Classifier. The notebook concludes that Logistic Regression with CountVectorizer and spaCy, and Naive Bayes Classifier with CountVectorizer and either NLTK or spaCy, perform best.
* **`fake_news_detection_app.ipynb`**: This Jupyter Notebook sets up and runs a Streamlit web application for interactive fake news detection. It uses `pyngrok` to create a public URL for the Streamlit app, allowing users to input text and get a prediction.

## How to use:

1.  **`fake_news_detection.ipynb`**:
    * Open the notebook in a Jupyter environment (e.g., Google Colab).
    * Run all cells to see the model training, evaluation, and the identified best-performing models.

2.  **`fake_news_detection_app.ipynb`**:
    * Open the notebook in a Jupyter environment (e.g., Google Colab).
    * Ensure you have `streamlit`, `pyngrok`, and `spacy` installed (`!pip install streamlit pyngrok -q`, `!pip install python -u spacy -q`, `!python -m spacy download en_core_web_lg`).
    * Set your `pyngrok` authentication token as instructed in the notebook.
    * Run the cells to start the Streamlit app. A public URL will be provided, which you can use to access the web application.

## Data Format:

Each sample in the training and testing datasets includes:
* The text of a tweet
* A keyword from the tweet (may be blank)
* The location from which the tweet was sent (may also be blank)

## Key Technologies:

* **Natural Language Processing (NLP)**: NLTK, spaCy
* **Machine Learning**: Logistic Regression, Naive Bayes Classifier
* **Vectorization**: CountVectorizer
* **Web Application**: Streamlit, pyngrok
