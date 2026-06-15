# Fake News Detection Using Machine Learning

## Project Overview

This project uses Natural Language Processing (NLP) and Machine Learning techniques to classify news articles as Real or Fake.

The workflow includes:

- Data Cleaning
- Text Preprocessing
- Stemming
- TF-IDF Vectorization
- Logistic Regression
- Naive Bayes Classification
- Model Evaluation
- Confusion Matrix Visualization

## Technologies Used

- Python
- Pandas
- NumPy
- NLTK
- Scikit-learn
- Matplotlib
- Seaborn

## Dataset

Dataset contains:

- Author
- Title
- News Label

Target Variable:

- 0 → Real News
- 1 → Fake News


## Workflow

### 1. Data Preprocessing

- Handle missing values
- Combine author and title columns
- Remove special characters
- Convert text to lowercase
- Remove stopwords
- Apply stemming

### 2. Feature Engineering

TF-IDF Vectorization is used to convert text into numerical features.

### 3. Model Training

#### Logistic Regression

- Max Iterations: 1000

#### Naive Bayes

- Multinomial Naive Bayes

### 4. Evaluation

Models are evaluated using:

- Accuracy Score
- Classification Report
- Confusion Matrix

## Results

| Model | Accuracy |
|---------|----------|
| Logistic Regression | ~98% |
| Naive Bayes | ~95% |

*(Results may vary slightly based on train-test split.)*

## Visualizations

- Model Accuracy Comparison
- Logistic Regression Confusion Matrix
- Naive Bayes Confusion Matrix


## How to Run

### Clone Repository

```bash
git clone https://github.com/yourusername/Fake-News-Detection.git
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Launch Notebook

```bash
jupyter notebook
```

Open:

```text
notebooks/Fake_News_Detection.ipynb
```

## Future Improvements

- Random Forest Classifier
- XGBoost
- Hyperparameter Tuning
- Streamlit Web App
- Deployment on Render/Heroku


## Author

Rutu Patel

Master's in Computer Science
