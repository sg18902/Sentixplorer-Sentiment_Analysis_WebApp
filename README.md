# SentimentExplorer

SentimentExplorer is an interactive web application designed for sentiment analysis of textual data. This intuitive tool allows users to input text and receive predictions on the sentiment expressed in that text. Whether it's customer reviews, social media posts, or any form of textual content, SentimentExplorer provides valuable insights into the emotions conveyed.

## Data and Model Overview

### Dataset

The SentimentExplorer web application was trained using a dataset of Twitter text samples. The dataset comprises tweets with associated sentiment labels, categorizing them as "Positive," "Negative," "Neutral," and "Irrelevant." The dataset was preprocessed to remove irrelevant information, handle missing values, and prepare the text for analysis.

Source: https://www.kaggle.com/datasets/jp797498e/twitter-entity-sentiment-analysis/

### Text Preprocessing

The text data underwent preprocessing, which involved the following steps:

1. **Stopword Removal**: Commonly used words (e.g., "the," "is," "in") that do not contribute much information for sentiment analysis were removed.

2. **Lemmatization**: Words were reduced to their base form (e.g., "running" to "run") to simplify analysis.

### Machine Learning Model

The web application employs a Multinomial Naive Bayes model for sentiment analysis. This choice was based on its effectiveness in text classification tasks, especially for datasets with a moderate to large number of features. The model was trained on the preprocessed text data.

### Feature Extraction

The text data was converted into numerical features using a Term Frequency-Inverse Document Frequency (TF-IDF) vectorizer. This technique transforms text data into a numerical format that can be used by machine learning algorithms.

### Model Performance

The model's performance was evaluated using metrics such as accuracy, precision, recall, and F1-score. These metrics provide insights into how well the model classifies text into different sentiment categories.

### Deployment

The trained model was integrated into a Flask web application, allowing users to input text for sentiment analysis. The web app provides a user-friendly interface for easy interaction.

### Future Improvements

In future iterations, the SentimentExplorer app could be enhanced by incorporating more advanced natural language processing techniques, exploring different machine learning algorithms, and expanding the dataset to improve accuracy and coverage across various types of textual data.

## Usage

1. Clone the repository.
2. Install the required libraries using `pip install -r requirements.txt`.
3. Run the Flask app using `python app.py`.
4. Open a web browser and go to `http://localhost:5000`.
5. Enter the text you want to analyze and click "Analyze".

## Technologies Used

- Python
- Flask
- HTML/CSS
- Bootstrap

## Acknowledgements

- The dataset used for training the model was sourced from https://www.kaggle.com/datasets/jp797498e/twitter-entity-sentiment-analysis/.


