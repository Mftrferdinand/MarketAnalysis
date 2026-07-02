# Data Sources & API Endpoints

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

## News (Google RSS)
```
python3 ~/.hermes/scripts/news_search.py "gold+XAUUSD+price+fed"
```

## BTC
```
https://api.coingecko.com/api/v3/simple/price?ids=bitcoin&vs_currencies=usd
https://query1.finance.yahoo.com/v8/finance/chart/BTC-USD?range=2mo&interval=1d
```

## Local Scripts
- News: ~/.hermes/scripts/news_search.py "keyword"
- Netflix: ~/.hermes/scripts/netflix_decode.py
- Monitor: ~/.hermes/scripts/monitor_xauusd.py
