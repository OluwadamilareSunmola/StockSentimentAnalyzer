# StockSentimentAnalyzer

## Description
StockSentimentAnalyzer is a Python-based tool that combines stock market data retrieval, sentiment analysis, and web scraping to analyze the sentiment of news articles related to specific stocks. Utilizing the `yfinance` library for financial data and `nltk`'s SentimentIntensityAnalyzer for sentiment analysis, this tool provides valuable insights into the market mood as reflected in the news.

## Features
- Retrieves current and historical stock data using `yfinance`.
- Scrapes news articles related to specific stock tickers.
- Performs sentiment analysis on the content of these articles.
- Calculates various stock-related metrics (e.g., price change, percent change).
- Flask web application for handling sentiment analysis requests.

## Installation
To get started, clone the repository and install the required dependencies.

```bash
git clone https://github.com/[OluwadamilareSunmola]/StockSentimentAnalyzer.git
cd StockSentimentAnalyzer
pip install -r requirements.txt
```

## Usage
To run the Flask application:

```bash
python app.py
```

The app will start on `localhost` at port `5000`. You can access the sentiment analysis feature through the endpoint `/sentiment` with a stock ticker as a query parameter.

Example:
```
http://localhost:5000/sentiment?ticker=AMZN
```

## API Reference
`GET /sentiment?ticker=<STOCK_TICKER>`
- Fetches sentiment analysis for the specified stock ticker.

## Contributing
Contributions are welcome! For major changes, please open an issue first to discuss what you would like to change.

## License
[MIT](https://choosealicense.com/licenses/mit/)

## Acknowledgements
- yfinance: For stock market data retrieval.
- NLTK: For sentiment analysis capabilities.
- BeautifulSoup: For web scraping functionalities.

