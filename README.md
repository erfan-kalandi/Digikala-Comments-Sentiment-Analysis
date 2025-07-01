# Digikala Comments Sentiment Analysis

This Jupyter notebook performs **sentiment analysis** on **Farsi (Persian)** product reviews from the Digikala e-commerce platform. It uses machine learning models to classify reviews as **positive** or **negative**, following text preprocessing, visualization, and feature engineering steps.

## Project Overview

The project includes the following key steps:

1. **Data Loading**

   * Loads a CSV file containing Digikala user comments and their associated sentiments.

2. **Text Preprocessing**

   * Persian-specific preprocessing using the `hazm` library:

     * Normalization
     * Tokenization
     * Stopword removal
     * Stemming (optional)
   * Removes non-Persian content, punctuation, digits, and extra whitespaces.

3. **Feature Extraction**

   * Applies **TFIDF Vectorization** to convert cleaned comments into numerical features.

4. **Model Training**

   * Trains and evaluates the following classifiers:

     * **Logistic Regression**
     * **Multinomial Naive Bayes**
     * **Random Forest**
   * Uses accuracy and confusion matrix for evaluation.

5. **Visualization**

   * Bar plots for sentiment distribution.
   * Word clouds for most frequent words in positive and negative reviews.

## Requirements

Install the following packages before running the notebook:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn hazm wordcloud
```

## Usage

1. Open the notebook:

```bash
jupyter notebook "Digikala Comments Sentiment Analysis.ipynb"
```

2. Run cells sequentially. The data file must be in the correct format, with at least the following columns:

   * `comment`: The review text
   * `label`: Sentiment label (0 = negative, 1 = positive)

3. Train and evaluate models. Output will include accuracy metrics and visualizations.

## Example Outputs

* **Sentiment distribution** bar chart
* **Confusion matrix** for model evaluations
* **WordClouds** showing most common positive/negative words


## File Structure

```plaintext
Digikala Comments Sentiment Analysis.ipynb  # Main notebook
data.csv                                    # Input data file
Report.pdf                                  # Persian report and readme
```

## 🔤 Language Considerations

This notebook is tailored for **Farsi** text using the `hazm` library, which handles Persian text normalization, stemming, and tokenization.

