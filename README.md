# Magic Formula Investment Screener

A simple web application that implements Joel Greenblatt's Magic Formula investment strategy to screen and rank stocks based on P/E ratio and ROIC.

## What is the Magic Formula?

The Magic Formula ranks companies by:
- **Low P/E Ratio** - cheaper stocks
- **High ROIC** - companies that use capital efficiently

Companies with the best combination of both metrics are ranked highest.

## Features

- **Real-time data** from multiple financial APIs (Alpha Vantage, Finnhub, Financial Modeling Prep)
- **Fallback data** ensures the app works even when APIs are unavailable
- **Historical backtesting** for 1, 3, and 5-year periods
- **Portfolio analysis** with different portfolio sizes (5, 10, 15, 20 stocks)
- **Interactive charts** showing performance vs S&P 500

## Quick Start

1. Open `index.html` in your web browser
2. View the automatically generated stock rankings
3. Use the backtest form to analyze historical performance
4. Click any company name to research on Google Finance

## API Setup (Optional)

For better data quality, add your API keys to `SimpleData.js`:

```javascript
const API_KEYS = {
    alphaVantage: 'YOUR_KEY_HERE',  // Get free key at alphavantage.co
    finnhub: 'YOUR_KEY_HERE',       // Get free key at finnhub.io
    fmp: 'YOUR_KEY_HERE'            // Get free key at financialmodelingprep.com
};
```

The app works fine with the default demo keys and fallback data.

## Files

- `index.html` - Main interface
- `SimpleData.js` - Core logic and data fetching
- `styles.css` - Styling
- `about.html` - Strategy explanation
- `API_SETUP.md` - Detailed API setup guide

## How to Use

1. **Rankings Table**: Shows companies ranked by Magic Formula score (lower is better)
2. **Backtest Form**: Test historical performance with your investment parameters
3. **Results**: View charts, statistics, and portfolio holdings over time

## Disclaimer

This is for educational purposes only. Always do your own research before making investment decisions.