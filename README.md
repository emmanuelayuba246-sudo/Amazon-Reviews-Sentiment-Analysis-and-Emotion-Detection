# Amazon Reviews Sentiment Analysis and Emotion Detection using NLP

## Project Overview

This project applies Natural Language Processing (NLP) techniques to analyze customer reviews from Amazon. The objective is to classify reviews into Positive, Negative, or Neutral sentiments, detect the emotions expressed in the reviews, and uncover customer opinions and trends that can support business decision-making.

The project demonstrates a complete NLP workflow, including data cleaning, text preprocessing, sentiment analysis, emotion detection, exploratory data analysis (EDA), visualization, and business insights.

---

## Objectives

- Clean and preprocess Amazon review data.
- Perform sentiment analysis using the VADER sentiment analyzer.
- Classify customer reviews as Positive, Negative, or Neutral.
- Detect emotions expressed in customer reviews using a pretrained NLP emotion classification model.
- Analyze sentiment patterns across customer ratings.
- Visualize findings using charts.
- Generate actionable business insights for marketing and product development.

---

## Dataset

The dataset contains Amazon customer reviews with the following information:

- Reviewer Name
- Country
- Review Date
- Rating
- Review Title
- Review Text
- Date of Experience

The analysis primarily focuses on the **Review Text** and **Rating** columns.

---

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Regular Expressions (re)
- NLTK (VADER Sentiment Analyzer)
- Hugging Face Transformers

---

## Project Workflow

### 1. Data Loading

- Imported the dataset into a Pandas DataFrame.
- Loaded the CSV file using the Python parsing engine.

### 2. Data Cleaning

- Removed rows containing missing review text.
- Removed missing rating values.
- Converted ratings into numeric format.
- Cleaned review text by:
  - converting text to lowercase
  - removing punctuation
  - removing numbers
  - trimming unnecessary spaces

### 3. Sentiment Analysis

Used the VADER SentimentIntensityAnalyzer from NLTK to calculate sentiment scores for each review.

Each review was classified as:

- Positive
- Negative
- Neutral

based on the compound sentiment score.

### 4. Emotion Detection

Applied a pretrained Hugging Face emotion classification model to identify emotions expressed in customer reviews.

Detected emotions include:

- Anger
- Fear
- Joy
- Sadness
- Surprise
- Disgust
- Neutral

### 5. Exploratory Data Analysis

Performed analysis including:

- Distribution of customer ratings
- Distribution of sentiments
- Comparison between customer ratings and predicted sentiment
- Emotion distribution

### 6. Visualization

Created visualizations to better understand customer opinions, including:

- Sentiment Distribution
- Rating vs Sentiment
- Emotion Distribution

---

## Results

The analysis revealed that:

- Most 1-star reviews were classified as Negative.
- Most 5-star reviews were classified as Positive.
- Some low-rated reviews were classified as Positive due to the limitations of lexicon-based sentiment analysis, where sarcasm, mixed opinions, and context are difficult to capture.
- Emotion detection showed that many negative reviews expressed emotions such as anger, fear, and sadness.

---

## Business Insights

The results can help businesses:

- Identify common customer frustrations.
- Monitor customer satisfaction.
- Improve products based on customer feedback.
- Support marketing decisions through sentiment trends.
- Detect emotional responses to products and services.

---

## Limitations

- Lexicon-based sentiment analysis may misclassify sarcastic or context-dependent reviews.
- Emotion detection using pretrained models may not always capture nuanced emotions accurately.
- Large transformer models require more computational resources for processing very large datasets.

---

## Future Improvements

- Perform aspect-based sentiment analysis.
- Build an interactive Power BI dashboard.
- Compare multiple sentiment analysis models.
- Train a custom machine learning model for improved sentiment classification.
- Analyze customer sentiment over time.

---

## Skills Demonstrated

- Data Cleaning
- Data Preprocessing
- Exploratory Data Analysis (EDA)
- Natural Language Processing (NLP)
- Sentiment Analysis
- Emotion Detection
- Data Visualization
- Business Insight Generation
- Python Programming

---

## Author

**Emmanuel Ayuba**
