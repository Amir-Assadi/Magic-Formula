# 🔑 API Setup for Real-Time Financial Data

To get current PE ratios and ROIC data instead of fallback data, you need to configure API keys in `SimpleData.js`.

## Quick Setup (5 minutes)

### 1. Alpha Vantage (Recommended - Most Reliable)
- **Free Tier**: 25 requests/day
- **Get Key**: https://www.alphavantage.co/support/#api-key
- **Setup**: Just enter email, get instant key
- **Replace in SimpleData.js**: Change `alphaVantage: 'demo'` to `alphaVantage: 'YOUR_KEY_HERE'`

### 2. Finnhub (High Rate Limit)
- **Free Tier**: 60 calls/minute (3,600/hour)
- **Get Key**: https://finnhub.io/register
- **Setup**: Quick email registration
- **Replace in SimpleData.js**: Change `finnhub: 'demo'` to `finnhub: 'YOUR_KEY_HERE'`

### 3. Financial Modeling Prep (High Daily Limit)
- **Free Tier**: 250 requests/day
- **Get Key**: https://financialmodelingprep.com/developer/docs
- **Setup**: Email registration required
- **Replace in SimpleData.js**: Change `fmp: 'demo'` to `fmp: 'YOUR_KEY_HERE'`

## Configuration

1. Open `SimpleData.js`
2. Find the `API_KEYS` section at the top
3. Replace `'demo'` with your actual API keys:

```javascript
const API_KEYS = {
    alphaVantage: 'YOUR_ALPHA_VANTAGE_KEY',
    finnhub: 'YOUR_FINNHUB_KEY', 
    fmp: 'YOUR_FMP_KEY'
};
```

## How It Works

- The app tries each API in order until it gets real data
- If all APIs fail, it falls back to cached data
- Green circle 🟢 = Real-time data
- Chart icon 📊 = Fallback data
- Hover over company names to see data source

## Recommended: Start with Alpha Vantage

Alpha Vantage is the most reliable and has comprehensive fundamental data. Even with just this one API key configured, you'll get real-time data for your Magic Formula rankings!
