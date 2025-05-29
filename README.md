# Cryptocurrency Market Analysis Toolkit

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-1.3%2B-orange)
![Seaborn](https://img.shields.io/badge/Seaborn-0.11%2B-red)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.4%2B-green)

A comprehensive Python toolkit for fetching and visualizing cryptocurrency market data from CoinMarketCap's API.

## Features

- **Real-time Data Fetching**: Pulls the latest market data for top 15 cryptocurrencies
- **Multi-dimensional Analysis**: 8 different visualization types for comprehensive market insights
- **Time-series Tracking**: Capable of running periodic updates to track market movements
- **Professional Visualizations**: Publication-ready charts with proper labeling and styling

## Visualization Suite

1. **Price Trends Over Time**
   - Tracks percentage changes across multiple timeframes (1h to 90d)
   - Highlights volatility patterns and relative performance

2. **Market Cap Distribution**
   - Pie chart showing market dominance
   - Side legend for clear labeling of all assets

3. **Liquidity Analysis**
   - Log-scale scatter plot of 24h volume vs price
   - Reveals market structure and trading activity

4. **Short-term Performance**
   - 24h and 7d percentage change comparisons
   - Identifies gaining and losing assets

5. **Tokenomics Analysis**
   - Circulating vs total supply comparisons
   - Fully diluted market cap evaluations

## Installation

```bash
pip install pandas seaborn matplotlib requests
```

## Configuration

1. Get a free API key from [CoinMarketCap Pro](https://pro.coinmarketcap.com/)
2. Replace the placeholder in the code:
```python
headers = {
  'X-CMC_PRO_API_KEY': 'your-api-key-here'
}
```

## Usage

Run the main script to:
1. Fetch latest market data
2. Generate all visualizations
3. Save results to CSV (optional)

```python
python crypto_analysis.py
```

## Example Outputs

![Market Cap Distribution](sample_images/market_cap_pie.png)
*Market dominance pie chart with side legend*

![Liquidity Analysis](sample_images/volume_vs_price.png)
*Log-log plot of trading volume vs price*

## Customization

Adjust these parameters as needed:
- `limit` in API call (default: 15 assets)
- Time intervals in `sleep()` for periodic updates
- Chart sizes and styling in `plt.figure()` calls

## Dependencies

- Python 3.8+
- pandas
- seaborn
- matplotlib
- requests
