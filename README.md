# Stock-Movement-Analysis-Based-on-Social-Media-Sentiment
---

# Reddit Stock Prediction

This project uses machine learning and sentiment analysis to predict stock trends based on discussions from Reddit. Specifically, data from Reddit is scraped, and sentiment analysis is applied to determine sentiment for Apple stock. We then correlate the sentiment data with Apple stock price changes obtained from Yahoo Finance to predict stock price movement.

## Overview

In this project, we achieved an **average accuracy of 80%** across various machine learning models for classifying Reddit discussions and predicting stock trends. The sentiment analysis was performed on scraped Reddit data (focused on Apple-related discussions), and stock data was obtained from Yahoo Finance. Several supervised learning models were applied, including:

- **Decision Tree**
- **Logistic Regression**
- **Naive Bayes**
- **Random Forest**

After performing sentiment analysis on the Reddit discussions, we correlated the sentiment data with Apple stock price changes. The **correlation matrix** obtained shows:

|                        | Lagged_Polarity | Price_Change |
|------------------------|-----------------|--------------|
| **Lagged_Polarity**     | 1.000000        | 0.082157     |
| **Price_Change**        | 0.082157        | 1.000000     |

The correlation of **0.082157** suggests a weak positive relationship between Reddit sentiment (Lagged Polarity) and Apple stock price changes, which limits the ability to make highly accurate predictions based solely on sentiment.

## How It Works

1. **Data Scraping**: Reddit discussions about Apple stock are scraped using the PRAW (Python Reddit API Wrapper).
2. **Sentiment Analysis**: Each Reddit post and comment is analyzed for sentiment (positive, negative, neutral) using sentiment analysis models.
3. **Machine Learning Models**: Several machine learning models (Decision Tree, Logistic Regression, Naive Bayes, Random Forest) are applied to predict stock trends based on sentiment.
4. **Stock Data**: Apple stock price data is fetched from Yahoo Finance.
5. **Correlation Analysis**: The correlation between sentiment data (Lagged Polarity) and Apple stock price changes is calculated to understand the relationship.
6. **Prediction**: Based on sentiment analysis and the correlation data, predictions are made about the direction of Apple stock prices.

## Results

- **Accuracy**: The average accuracy of all models is **80%**, based on the classification of sentiment and prediction of stock trends.
- **Correlation**: A **correlation of 0.082157** between **Lagged Polarity** (sentiment) and **Price Change** was observed, indicating a weak positive relationship. This suggests that while sentiment may have some effect, it is not a strong predictor of stock price movement on its own.
- **Prediction**: Sentiment analysis and correlation with stock prices enabled us to forecast stock price movements with moderate accuracy, but further improvements can be made by incorporating additional features or using more sophisticated models.

## Usage

To use the model:

1. Scrape Reddit discussions related to Apple using the provided script.
2. Perform sentiment analysis on the scraped data.
3. Train the machine learning models (Decision Tree, Logistic Regression, Naive Bayes, Random Forest) on the sentiment data.
4. Fetch historical Apple stock price data from Yahoo Finance.
5. Calculate the correlation between the sentiment data and stock price changes.
6. Use the correlation and model predictions to predict future stock trends based on Reddit sentiment.

This model can be used to analyze how social media sentiment might influence stock price movement, particularly for Apple.

## Authors

- **Rishabh Paraswani**

## Documentation

A preprint of the research is available on SSRN.

## Feedback

If you have any feedback, please reach out to me at **rishiparaswani@gmail.com**.

Feel free to file a new issue with a respective title and description on the **Reddit Stock Prediction** repository. If you’ve already found a solution to your problem, I would love to review your pull request!

---

