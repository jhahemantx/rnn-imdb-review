# IMDB Movie Review Sentiment Analysis

## Overview
This project is an IMDB movie review sentiment analysis application using an RNN model in TensorFlow. It predicts whether a given movie review is **Positive** or **Negative** based on trained sentiment analysis models.

## Features
- Uses a **Simple RNN** model trained on the IMDB dataset.
- Preprocesses text input by tokenizing and padding sequences.
- Provides real-time predictions via a **Streamlit** web app.
- Displays sentiment prediction along with a confidence score.


## Installation
To set up the environment, install the required dependencies:
```bash
pip install tensorflow numpy streamlit
```

## Usage
### Running the Web Application
To launch the Streamlit app:
```bash
streamlit run app.py
```
Then, open `http://localhost:8501/` in your browser.

### Predicting Sentiment
1. Enter a movie review in the text area.
2. Click the **"Classify"** button.
3. The model predicts whether the review is **Positive** or **Negative** and displays the confidence score.

## Model Details
- **Dataset:** IMDB Movie Reviews dataset.
- **Model Type:** Simple RNN.
- **Preprocessing:**
  - Tokenization using Keras' `imdb.get_word_index()`.
  - Padding sequences to a fixed length of 500.
- **Prediction Mechanism:**
  - Converts input text into numerical sequences.
  - Feeds sequences into the pre-trained RNN model.
  - Outputs a sentiment classification with a confidence score.

## Future Enhancements
- Upgrade to **LSTM or GRU** for better sentiment analysis.
- Improve preprocessing using **stemming/lemmatization**.
- Deploy the model as a **Dockerized web service**.
- Enhance UI with **interactive visualizations**.


