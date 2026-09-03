# Finance News Sentiment vs Share Price Analyzer

A Python tool that compares news sentiment for a company against its share price movement, using Goldman Sachs (GS) and Deutsche Bank (DB) as examples.

## What it does
- Pulls recent news headlines for each company from Google News RSS
- Scores each headline's sentiment using VADER sentiment analysis
- Pulls recent share price history using yfinance
- Plots sentiment score against share price over time to see if they move together

## Why I built this
I'm interested in how AI is being used in financial operations, particularly around automating data-driven decision support. This project was a way to practically explore sentiment analysis and financial data together on a small scale.

## Tech used
- Python
- VADER (sentiment analysis)
- yfinance (stock price data)
- pandas (data handling)
- matplotlib (visualisation)

## How to run it
1. Clone this repo
2. Install dependencies: `pip install -r requirements.txt`
3. Run the script: `python3 sentiment_stock_analyzer.py`
4. Charts are saved as PNG files in the same folder

## Example output
The script generates a chart for each company showing daily average sentiment score plotted against closing share price over a 2-week period.

## Limitations
VADER is a general-purpose sentiment tool, not finance-specific, so it can miss nuance in financial language (e.g. "faces regulatory scrutiny" may score as neutral when it's actually negative for markets). A next step would be testing a finance-tuned sentiment model for comparison.
