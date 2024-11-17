    # potfolio_optimization
Collection of different ML based strategies for optimal strategies using technical data (price-volume) and fundamental data

# Description
This repository contains various Jupyter notebooks focused on different aspects of financial data analysis, machine learning models/techniques (GNN, LLM, RAG, KG), and data processing techniques. Below is a brief description of each notebook:

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

* **Aug 2024** - Worked on `backtest_aug24.ipynb` & `pdf_analyzer.ipynb`
    * Explored VectorBT and backtesting.py
    * Used Binance BTC data.
    * Also used YFC modeule in vbt to realtime download data
    * Generated heatmap based on RSI entries (~35) and exit (~70)
    * Utilized Large Language Model (Llama 3.1) to categorize personal expense transactions.
        * Additionally, employed the same LLM for Retrieval-Augmented Generation (RAG) using personal documents.
        * Used Ollama for model orchetration.
 
* **Sep 2024**
    * Explored Graph Neural networks (GNN) for Top 10 ETFs in NYSE.
    * Tested several spatio-temporal GNNs with ime-series data
        * Focus on the the edge relationships between the ETF nodes to understand inter-dependency
        * Also explore the dynamic nature of the graphs with ETFs egde characteristics varying at different time periods.
    * Extended the work on LLM through populating a Knowledge Graph (KG) and then using it for RAG

* **Oct 2024**
    * Working on combining the knowledge graph and inference from GNN through a LLM (multi-model knowledge distilation).
    * Improving the spatio-temporal GNN
    * Exploring Llama 3.2

* **Nov 2024**
    * Extarcted embdeded text from podcast and yt videos
    * Exploring Llama 3.2 Multi-modal LLMs - 11B
    * Building LLM from scratch
