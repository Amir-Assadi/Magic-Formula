# Magic Formula Stock Screener

A simple web app for ranking stocks using Joel Greenblatt's Magic Formula.

## Features

- Ranks stocks by P/E Ratio and ROIC
- Real-time data from Alpha Vantage API (with your API key)
- Simple backtest analysis
- Works with demo/fallback data if no API key

## How to Use

1. Place all files (`index.html`, `SimpleData.js`, `styles.css`) in the same folder.
2. Open `index.html` in your browser.
3. View the stock rankings table and use the backtest form.

## API Setup

To use live data, get a free API key from [Alpha Vantage](https://www.alphavantage.co/support/#api-key) and update this line in `SimpleData.js`:

```javascript
const API_KEY = 'YOUR_API_KEY_HERE';
```

## Disclaimer

This app is for educational purposes only.  
Always do your own research before investing.
