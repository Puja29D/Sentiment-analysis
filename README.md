*Sentiment Analysis*

This project focuses on performing Sentiment Analysis on text data using Natural Language Processing (NLP) and Machine Learning techniques.
The goal was to clean the text, convert it into numerical features, train a classification model, and visualize key patterns in the data.
Project Overview

The project includes:

Dataset exploration

Text cleaning & preprocessing

Feature engineering using TF-IDF

Train–test split

Naive Bayes model training

Model evaluation

Data visualization

Word cloud generation

This workflow helps convert raw text into structured insights.

🛠️ Steps Performed
1️⃣ Data Import & Initial Exploration

To understand the dataset, I imported all required Python libraries and explored the data using:

head()

info()

data.columns

describe()

isnull().sum()

This helped identify missing values, check data types, and understand the structure of the dataset.

2️⃣ Handling Missing Values

All missing values were replaced with the text:

"missing"


This prevents null entries from causing issues during preprocessing or model training.

3️⃣ Text Cleaning & Preprocessing

To prepare the text for modeling, I applied several NLP cleaning steps:

Converted text to lowercase

Removed links, mentions, hashtags, and symbols

Removed extra spaces

Converted words to their base form (lemmatization/stemming)

This ensures clean and consistent text for feature extraction.

4️⃣ Feature Engineering – TF-IDF Vectorization

Used TF-IDF Vectorizer from Scikit-learn to convert text into numerical values based on term importance.

TF-IDF helps highlight meaningful words while reducing the impact of frequently repeated terms.

5️⃣ Train–Test Split

80% of the data used for training

20% used for testing

This helps evaluate how well the model performs on unseen data.

6️⃣ Model Training – Naive Bayes

Trained a Naive Bayes classifier using the TF-IDF features.

Printed performance metrics (accuracy, classification report) to evaluate model quality.

7️⃣ Data Visualization

Created:

Bar chart showing the number of samples in each sentiment category
→ Helps identify class balance or imbalance

8️⃣ Word Cloud Visualization

Generated two separate word clouds:

Positive sentiment word cloud

Negative sentiment word cloud

These visually highlight the most frequent words used in each sentiment group.

📈 Final Output

The final output includes:

A cleaned and processed dataset

A trained Naive Bayes sentiment classification model

Visual insights through bar charts and word clouds

Performance metrics to evaluate model effectiveness

🧰 Tech Stack Used

Python,
Pandas / NumPy,
NLTK / re (text preprocessing),
Scikit-learn,
Matplotlib / Seaborn,
WordCloud library,
Google Colab.
