# Data Sources

## Gold Spot (XAUUSD)
- **gold-api.com**: `https://api.gold-api.com/price/XAU` — returns JSON `{"price": 1234.56}`
- **fxratesapi**: `https://api.fxratesapi.com/latest?base=XAU&symbols=USD` — returns JSON with rates

## Gold Futures (GC=F)
- **Yahoo Finance**: `https://query1.finance.yahoo.com/v8/finance/chart/GC=F?range=2mo&interval=1d` — daily OHLCV for 2 months
- **Yahoo Finance hourly**: `https://query1.finance.yahoo.com/v8/finance/chart/GC=F?range=5d&interval=1h` — hourly OHLCV for 5 days

## Fear & Greed Index
- **alternative.me**: `https://api.alternative.me/fng/?limit=1` — returns JSON `{"data":[{"value":"11","value_classification":"Extreme Fear"}]}`

## News
- **Google News RSS**: `https://news.google.com/rss/search?q=gold+XAUUSD+price+fed&hl=en-US&gl=US&ceid=US:en` — returns XML feed
- **News scraper script**: `~/.hermes/scripts/news_search.py` — searches Google News RSS and returns top headlines with links

## Economic Calendar
- **Investing.com**: `https://www.investing.com/economic-calendar/` — upcoming events (FOMC, NFP, CPI)
- **ForexFactory**: `https://www.forexfactory.com/calendar.php` — economic calendar

## Bitcoin (BTC)
- **CoinGecko**: `https://api.coingecko.com/api/v3/coins/bitcoin` — full market data
- **CoinGecko price**: `https://api.coingecko.com/api/v3/simple/price?ids=bitcoin&vs_currencies=usd` — simple price
- **CoinGecko OHLCV**: `https://api.coingecko.com/api/v3/coins/bitcoin/ohlc?vs_currency=usd&days=30` — 30-day OHLCV
- **CoinGecko chart**: `https://api.coingecko.com/api/v3/coins/bitcoin/market_chart?vs_currency=usd&days=30` — 30-day market chart