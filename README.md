# Sentiment Analysis on Reddit and eBay Data

This project performs sentiment analysis on Reddit and eBay data using pre-trained BERT and RoBERTa models. The analysis includes data collection, cleaning, sentiment classification, and performance evaluation.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Models Used](#models-used)
- [Data Collection](#data-collection)
- [Data Cleaning](#data-cleaning)
- [Sentiment Analysis](#sentiment-analysis)
- [Evaluation](#evaluation)
- [Results](#results)

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/yourrepository.git
    cd yourrepository
    ```

2. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

3. Download NLTK resources:
    ```python
    import nltk
    nltk.download('punkt')
    nltk.download('stopwords')
    ```

## Usage

1. Open the Jupyter notebook:
    ```sh
    jupyter notebook work.ipynb
    ```

2. Run the cells in the notebook to perform sentiment analysis on Reddit and eBay data.

## Project Structure

- `work.ipynb`: The main Jupyter notebook containing the code for data collection, cleaning, sentiment analysis, and evaluation.
- `requirements.txt`: The list of required packages.
- `README.md`: This README file.

## Models Used

- **BERT**: `nlptown/bert-base-multilingual-uncased-sentiment`
- **RoBERTa**: `cardiffnlp/twitter-roberta-base-sentiment`

## Data Collection

Reddit data is collected using the PRAW library. The `collect_reddit_data` function fetches posts based on a keyword.

## Data Cleaning

Text data is cleaned using NLTK. The `clean_text` function tokenizes the text, removes stopwords, and retains only alphabetic tokens.

## Sentiment Analysis

Sentiment analysis is performed using pre-trained BERT and RoBERTa models. The `analyze_sentiment_bert` and `analyze_sentiment_roberta` functions classify the sentiment of the cleaned text.

## Evaluation

The performance of the models is evaluated using accuracy, precision, recall, and F1 score. The `evaluate_performance` function calculates these metrics.

## Results

The notebook provides the overall sentiment score and classification for the collected Reddit data. It also evaluates the performance of the models on a labeled eBay dataset.

## Example Output

```plaintext
Input = iphone 14

Collecting Reddit data...
Collected 234 Reddit posts

Cleaning Reddit data...

Performing sentiment analysis with BERT model...

The overall sentiment score: -0.008122405478070116
The overall sentiment classified: Neutral
```

