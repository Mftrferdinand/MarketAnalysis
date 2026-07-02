# Data Sources & API Endpoints

**CRITICAL: Minimum 3-4 cross-checked, interrelated & trusted sources for Fundamental section. NOT just Forex Factory alone.**

## Gold Spot
```
https://api.gold-api.com/price/XAU
```

## FX Rate (fallback)
```
https://api.fxratesapi.com/latest?base=XAU&currencies=USD
```

## Gold Futures — Daily (2mo)
```
https://query1.finance.yahoo.com/v8/finance/chart/GC=F?range=2mo&interval=1d
```

## Gold Futures — Hourly (5d)
```
https://query1.finance.yahoo.com/v8/finance/chart/GC=F?range=5d&interval=1h
```

## DXY Index
```
https://query1.finance.yahoo.com/v8/finance/chart/DX-Y.NYB?range=1d&interval=1m
```

## BTC / Crypto (CoinGecko)
```
https://api.coingecko.com/api/v3/simple/price?ids=bitcoin&vs_currencies=usd
https://api.coingecko.com/api/v3/coins/bitcoin/ohlc?vs_currency=usd&days=30
https://query1.finance.yahoo.com/v8/finance/chart/BTC-USD?range=2mo&interval=1d
```

## Economic Calendar (Forex Factory)
```
https://nfs.faireconomy.media/ff_calendar_thisweek.json
```
- Use for: NFP, FOMC, CPI, high-impact events
- Verify event dates/times — never guess

## Fundamental News Sources (Cross-check 3-4 REQUIRED)

1. **Forex Factory Calendar** — Economic events & data releases
   - API: `nfs.faireconomy.media/ff_calendar_thisweek.json`
   - Check before every analysis for upcoming catalysts

2. **Investing.com / TradingView** — Price overview, technicals, economic calendar
   - Use for: cross-checking price levels, technical confirmations, event schedules

3. **Reuters / Bloomberg / CNBC** — Global macro news
   - Use for: Fed policy statements, geopolitical developments, inflation/treasury data
   - Search via Google News RSS with specific keywords

4. **Google News RSS** — Broad news aggregation
   ```
   python3 ~/.hermes/scripts/news_search.py "gold+XAUUSD+price+fed"
   python3 ~/.hermes/scripts/news_search.py "bitcoin+BTC+crypto+fed"
   ```
   - Use for: real-time news headlines, event coverage, market sentiment drivers

**Cross-check rule:** Before writing the Fundamental section, verify key facts (event dates, data figures, policy statements) across at least 3 of these sources. Never rely on a single source alone.

## Local Scripts
- News: ~/.hermes/scripts/news_search.py "keyword"
- Netflix: ~/.hermes/scripts/netflix_decode.py
- Monitor: ~/.hermes/scripts/monitor_xauusd.py
