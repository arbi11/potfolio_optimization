    # potfolio_optimization
Collection of different strategies for optimal strategies using technical data (price-volume) and fundamental data

# Description
This repository contains various Jupyter notebooks focused on different aspects of financial data analysis, machine learning models, and data processing techniques. Below is a brief description of each notebook:

## Getting Started
To get started with these notebooks, clone the repository and ensure you have the necessary dependencies installed. Each notebook may have specific requirements, so please refer to the comments within each notebook for detailed instructions.

```
git clone <repository_url>
cd <repository_directory>
pip install -r requirements.txt
```


## Contributing
Contributions are welcome! Please fork the repository and submit a pull request with your changes.

## License
This project is licensed under the MIT License


# Development
* **June 2024**
    * Worked on `P1_P6.ipynb`
        * Used `yfinance` & `pandas_datareader` for downloading data.
        * Scrapped `BeautifulSoup4` & `requests` to download S&P 500 data.
            * Used bs4 to get all tickers from wikipedia
        * Basic data manipulation
            * Moving (rolling) average
            * Candlestick (from `mplfinance`) based on OHLC
    * On `P7-P10.ipynb`
        * Correlation analysis
        * Data pre-processing for Machine Learning algos. 

* **July 2024** - Worked on `zipline_ingest_data_alpha_factors.ipynb`
    *  Explored `Zipline - Reloaded`
        * CLI
        * Notebook magic commands
        * python API
    * Documented instructions to run zipline on CLI
    * Portfolio Optimization
        * Mean Reversion
        * 5 factor pipeline analysis

* **Aug 2024** - Worked on `backtest_aug24.ipynb`
    * Explored VectorBT and backtesting.py
    * Used Binance BTC data.
    * Also used YFC modeule in vbt to realtime download data
    * Generated heatmap based on RSI entries (~35) and exit (~70)
