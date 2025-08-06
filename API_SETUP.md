# Alpha Vantage API Setup

To use live stock data:

1. Visit [Alpha Vantage](https://www.alphavantage.co/support/#api-key) and request a free API key.
2. Open `SimpleData.js` in your project folder.
3. Find this line:
   ```javascript
   const API_KEY = 'demo';
   ```
4. Replace `'demo'` with your API key:
   ```javascript
   const API_KEY = 'YOUR_API_KEY_HERE';
   ```
5. Save the file and reload `index.html` in your browser.

**Note:**  
If you use `'demo'`, the app will show fallback data for most stocks.
