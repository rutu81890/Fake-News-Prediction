# Fake News Prediction
A machine learning project that detects fake news articles using Natural Language Processing (NLP) and Logistic Regression. The model analyzes the author and title of a news article to classify it as Real or Fake.

How It Works

Data Loading – Loads a labeled news dataset (train.csv)
Preprocessing – Combines author + title into a single content field
Text Stemming – Removes stopwords and stems words using NLTK's PorterStemmer
TF-IDF Vectorization – Converts text into numerical feature vectors
Model Training – Trains a Logistic Regression classifier
Evaluation – Reports accuracy, classification report, and confusion matrix
Prediction – Predicts whether a custom news headline is real or fake

Project Structure

fake-news-prediction/
- Fake_News_Prediction.ipynb   # Main Jupyter Notebook
- train.csv                    # Dataset (not included — see below)
- requirements.txt             # Python dependencies
- .gitignore                   # Files to exclude from Git
- README.md                    # Project documentation


Dataset

This project uses the Fake News dataset from Kaggle:
🔗 https://www.kaggle.com/c/fake-news/data

Download train.csv and place it in the root of this project folder.

ColumnDescriptionidUnique ID for each articletitleHeadline of the news articleauthorAuthor of the articletextFull article bodylabel0 = Real News, 1 = Fake News


Installation

1. Clone the repository

bashgit clone https://github.com/YOUR_USERNAME/fake-news-prediction.git
cd fake-news-prediction

2. Install dependencies

bashpip install -r requirements.txt

3. Download the dataset

Download train.csv from Kaggle and place it in the project folder.

4. Run the notebook

bashjupyter notebook Fake_News_Prediction.ipynb


Results

MetricScoreTraining Accuracy~98%Testing Accuracy~97%

The model outputs a confusion matrix heatmap using Seaborn for visual evaluation.

Tech Stack

Tool / LibraryPurposePythonCore programming languagePandas & NumPyData manipulationNLTKText preprocessing & stemmingScikit-learnTF-IDF vectorization & modelMatplotlib/SeabornVisualizationJupyter NotebookInteractive development

Example Prediction

pythonnews = ["Breaking: Government announces new economic reforms"]
news_vector = vectorizer.transform(news)
prediction = model.predict(news_vector)

if prediction[0] == 0:
    print("Real News")
else:
    print("Fake News")


