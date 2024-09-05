# IMDb Movie Review Sentiment Analysis Using NLP

This project is a sentiment analysis of IMDb movie reviews using a Kaggle dataset and Natural Language Processing (NLP) techniques. It aims to classify reviews as either positive or negative using a Random Forest classifier.

## Project Overview

The project involves:
1. Cleaning the data by removing HTML tags, punctuation, numbers, and stopwords.
2. Converting the cleaned text into a numeric format using Bag of Words (CountVectorizer).
3. Training a Random Forest classifier to predict the sentiment of movie reviews.

## Dataset

The dataset used for this project is labeled IMDb movie reviews from Kaggle. It contains 25,000 reviews with sentiments labeled as:
- 1 for positive reviews
- 0 for negative reviews

**Important:** After downloading the repository, please append the data from `NLPlabeledData2.tsv` to the end of `NLPlabeledData.tsv` before running the project. This step is essential for the proper functioning of the model.

## Installation & Usage

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/your-repo-name.git
```

### 2. Install dependencies
Make sure you have nltk, scikit-learn, pandas, matplotlib, BeautifulSoup4, and numpy installed. You can install them using the following command:

```bash
pip install -r requirements.txt
```

### 3. Download NLTK stopwords
Run the following Python command to download the necessary NLTK data:

```python
import nltk
nltk.download('stopwords')
```

### 4. Prepare the dataset
Ensure the dataset is in the correct format:

Append the contents of NLPlabeledData2.tsv to NLPlabeledData.tsv to include all necessary data.

### 5. Run the project
To train the model and test the sentiment analysis, run:

```bash
python sentiment_analysis.py
```

### 6. Example Usage
You can test the model with a custom comment:

```python
new_comment = "This movie was Terrible"
predict = model.predict(new_comment)
print("Sentiment:", "Positive" if predict == 1 else "Negative")
```
