# TrinityTrend

TrinityTrend is a modular, multi-signal trading indicator designed for clarity, conviction, and volatility awareness. It blends:

- Candle TrendStrength (normalized directional scoring)
- SuperTrend overlay (bias and trailing stop logic)
- TTM Squeeze detection (volatility compression and breakout timing)

Built for traders across all timeframes—from scalpers to macro strategists.

---

## Core Logic

### TrendStrength Index
- Combines Price Change, EMA Slope, and MA Distance
- Normalized to a -100 to +100 scale
- Color-coded candles: bullish, bearish, neutral

### SuperTrend Overlay
- Independent mode selection (Intraday, Swing, Macro, Extended Macro)
- Factor and ATR tuned per mode
- Acts as bias filter and trailing stop

### TTM Squeeze Detection
- Bollinger Bands vs. Keltner Channels
- Auto-configured per mode
- Highlights volatility compression zones

---

## Mode Profiles

| Mode            | Lookback | MA Type     | ATR | Squeeze Settings | Use Case                          |
|-----------------|----------|-------------|-----|------------------|-----------------------------------|
| Intraday        | Short    | EMA/EMA     | 10  | Default           | Scalps, quick reversals           |
| Swing           | Medium   | EMA/SMA     | 14  | Default           | Multi-day trend capture           |
| Macro           | Long     | SMA/SMA     | 20  | BB: 30/2.5, KC: 30/1.8 | Bull/bear phase tracking     |
| Extended Macro  | Very Long| SMA/SMA     | 50  | BB: 50/3.0, KC: 50/2.0 | Institutional cycle alignment |

---

## Modular Design

- Mix and match TrendStrength and SuperTrend modes
- Example: Intraday candles inside Extended Macro bias
- Supports multi-timeframe overlays and strategic forks

<img width="1753" height="753" alt="TTM Squeez" src="https://github.com/user-attachments/assets/566dd138-e2bd-44a2-ba95-490490a2976c" />
