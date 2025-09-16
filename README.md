# Private Equity Sentiment Analysis

This repository contains a notebook that gathers, preprocesses, and analyzes recent news articles related to private equity and global financial topics. The workflow includes scraping data, cleaning text, extracting features, and scoring sentiment, culminating in the classification of articles as positive, neutral, or negative.[1]

## Features

- **Automated news collection:** Retrieves articles from multiple sources, including DW, ABC News, BBC, Al Jazeera, and The Washington Post.[1]
- **Text cleaning & processing:** Converts titles and content to lowercase, removes punctuation and special characters, tokenizes, and cleans for modeling.[1]
- **Sentiment analysis:** Computes scores for each article and categorizes them into positive, neutral, or negative classes.[1]
- **Metadata enrichment:** Each news item includes source, image, date, and links for reference.[1]

## Getting Started

### Prerequisites

- Python 3.8+
- Jupyter Notebook
- Recommended: pandas, numpy, requests, nltk, scikit-learn

### Usage

1. Clone this repository:

   ```bash
   git clone https://github.com/your-username/private-equity-sentiment.git
   ```
2. Install required packages:

   ```bash
   pip install pandas numpy requests nltk scikit-learn
   ```
3. Launch the notebook:

   ```bash
   jupyter notebook Private_Equity.ipynb
   ```
4. Follow the included workflow to process articles and analyze sentiment.[1]

## Dataset Structure

| Column               | Description                                 |
|----------------------|---------------------------------------------|
| guid                 | Article identifier                          |
| image                | Link to representative image                |
| link                 | Article link                                |
| publishedAt          | Publication date/time                       |
| source               | News outlet name                            |
| title                | Original article headline                   |
| lowercase_text       | Headline in lowercase                       |
| no_special_chars     | Punctuation-free headline                   |
| tokenized_text       | Tokenized words from headline               |
| text_cleaned         | Cleaned tokens after stopword removal       |
| text_cleaned_joined  | Cleaned tokens put together as text         |
| sentiment_score      | Numeric sentiment value [-1, 1]             |
| sentiment_category   | Labeled class: Negative, Neutral, Positive  |

## Contributing

Questions, suggestions, and pull requests to improve processing or expand features are welcome.
