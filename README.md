# OKX Crypto Trading Monitor (Raspberry Pi 5)

Real-time cryptocurrency trading data collector from **OKX WebSocket API** running on **Raspberry Pi 5**. Processes 8 crypto pairs (BTC, ETH, SOL, etc.) with **moving averages**, **Pearson correlations**, and **performance monitoring**.

## 🎯 Features
- **Live WebSocket** connection to OKX (8 pairs: BTC-USDT, ETH-USDT, etc.)
- **15-min Moving Averages** + total volume per minute
- **Pearson Correlation** between all instrument pairs (saved to CSV)
- **High-resolution timestamps** (`clock_gettime`)
- **Multi-threading**: Data collection, MA computation, correlation threads
- **Performance logging**: CPU idle %, processing delays, timing diffs
- **ARM64 cross-compilation** for Raspberry Pi 5 (Debian Bookworm)
