# Hate Speech Detection System

This project focuses on detecting hate speech in text using machine learning. It leverages a decision tree classifier to predict whether a given text is categorized as hate speech, offensive language, or neither. The project includes data preprocessing techniques, feature extraction, and a simple web-based user interface for predictions using Streamlit.

## Project Structure

- *hatespeech.py*: The main script that handles data preprocessing, model training, and the web-based prediction interface using Streamlit.
  
## Features

1. *Data Preprocessing*:
   - Cleaning text data by removing URLs, special characters, punctuation, and stopwords.
   - Applying stemming to reduce words to their base forms using the NLTK library.
   
2. *Feature Extraction*:
   - Using CountVectorizer to convert text data into numerical features suitable for machine learning models.
   
3. *Model Training*:
   - A DecisionTreeClassifier from sklearn is trained on labeled Twitter data to predict whether a tweet contains hate speech, offensive language, or neither.

4. *Web Interface*:
   - The project uses Streamlit to provide a simple user interface where users can input a tweet, and the model will classify it as hate speech, offensive language, or neither.
   
## Dependencies

Make sure to install the required libraries before running the project:

- nltk
- pandas
- numpy
- scikit-learn
- streamlit

You can install the dependencies using:

bash
pip install -r requirements.txt


## How to Run

1. Clone this repository:
   bash
   git clone https://github.com/yourusername/hate-speech-detection.git
   cd hate-speech-detection
   

2. Install the dependencies:
   bash
   pip install -r requirements.txt
   

3. Download the NLTK stopwords data (if not already installed):
   python
   import nltk
   nltk.download('stopwords')
   

4. Run the Streamlit app:
   bash
   streamlit run hatespeech.py
   

5. The app will be available at http://localhost:8501/ where you can input tweets and get predictions.

## Dataset

The project utilizes a Twitter dataset with labeled tweets for:
- Hate Speech
- Offensive Language
- No Hate or Offensive Language

## Functionality

1. *Text Preprocessing*:
   - The script includes functions to clean and stem the input text.
   
2. *Model Training*:
   - A decision tree classifier is used to train the model on the preprocessed text data.
   
3. *Prediction*:
   - The user inputs a tweet, and the model classifies the tweet into one of the three categories.
