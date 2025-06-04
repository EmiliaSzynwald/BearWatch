# BearWatch
BearWatch is a web-based application that delivers real-time stock market data, dynamic trend charts, and the latest financial news. Designed for U.S. market participants, BearWatch empowers users to explore stocks, indices, and market headlines through an intuitive, responsive dashboard. The platform aggregates data from Yahoo Finance (via yfinance), updating visualizations and news feeds in real time to ensure users always have the latest market insights at their fingertips.

## Features

- **Live Market Data:** Real-time price quotes, trend charts, and key statistics for U.S. stocks and indices (S\&P 500, Nasdaq, Dow Jones).
- **Interactive Visualizations:** Dynamic charts with hoverable details, interval selection (1-day, 5-day, 1-month, etc.), and responsive updates.
- **Trending Stocks:** Instantly view and explore the most active and trending stocks.
- **Comprehensive Stock Pages:** Detailed stock profiles with statistics, company info, related news, and similar stock recommendations.
- **News Aggregation:** Financial news headlines and articles, sorted in reverse chronological order, both market-wide and stock-specific.
- **Search Functionality:** Fast, auto-complete search for stocks by name or ticker symbol.
- **Accessibility:** Colorblind-friendly chart modes and adjustable UI for enhanced visibility.
- **No Registration Required:** All features available to unregistered users—no account or authentication needed.
- **Cross-Platform:** Runs on all modern browsers and devices with an internet connection.

## Technology Stack

- **Backend:** Python 3.11+, Flask, Dash
- **Frontend:** Dash, Plotly, HTML, CSS
- **Data APIs:** [yfinance](https://yfinance-python.org/reference/index.html) (Yahoo Finance)
- **Data Processing:** Pandas
- **Version Control:** GitHub

## Usage

- **Home Page:** View trending stocks, market indices graphs, and latest news.
- **Search:** Use the search bar on any page to look up stocks by name or ticker.
- **Stock Pages:** Click a stock to see its detailed chart, statistics, news, and recommendations.
- **News Page:** Access market-wide headlines and search for news relevant to specific stocks.
- **Accessibility:** Use the accessibility button to adjust color schemes for colorblind modes.

## System Architecture

BearWatch follows a **Model-View-Controller (MVC)** architecture:


| Layer | Description |
| :-- | :-- |
| Model | Fetches and processes data from yfinance and News API; manages data structures (Pandas DataFrames, dictionaries). |
| View | Renders interactive charts, dashboards, and UI components using Dash, Plotly, HTML, and CSS. |
| Controller | Handles user input, API requests, and updates views in real time via Flask routes and Dash callbacks. |

**Key Patterns:**

- Observer (real-time updates), Repository (data access), Singleton (server instance), Facade (API abstraction).

**Authors:**
Aisha Ahmad, Jared Bergenstock, Owen Byron, Joel David, Irene Paul, Emilia Szynwald
