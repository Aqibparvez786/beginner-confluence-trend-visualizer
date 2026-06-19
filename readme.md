# Beginner Confluence Trend Visualizer (BCTV)

A clean, beginner-friendly **Pine Script v6** indicator designed for TradingView. It combines a Trend Filter (Simple Moving Average) with a Momentum Oscillator (Relative Strength Index) to identify high-probability pullback zones (Buying the Dip in an Uptrend, Selling the Rally in a Downtrend).

## 🚀 Features

- **Trend Filtering:** Uses a customizable Simple Moving Average (SMA) to determine overall market direction.
- **Pullback Identification:** Leverages the Relative Strength Index (RSI) to find temporary overbought or oversold conditions within a larger trend.
- **Visual Signals:** 
  - Green/Red triangles (`BUY` / `SELL`) plotted directly on the chart.
  - Optional translucent background highlights to mark specific trading zones.
- **On-Chart Status Dashboard:** A sleek table in the top-right corner displaying the current Trend, exact RSI value, and active Signal state.
- **Alerts Ready:** Includes pre-configured alert conditions for seamless integration with TradingView alerts.

## 🛠️ How It Works (Confluence Logic)

The indicator looks for two specific scenarios to generate signals:

1. **Bullish Confluence (BUY DIP):**
   - **Condition:** Price is **above** the SMA (Uptrend) **AND** the RSI is **below** the Oversold level (e.g., 30).
   - **Concept:** Buying a temporary oversold dip during a strong macro uptrend.

2. **Bearish Confluence (SELL RALLY):**
   - **Condition:** Price is **below** the SMA (Downtrend) **AND** the RSI is **above** the Overbought level (e.g., 70).
   - **Concept:** Shorting a temporary overbought rally during a macro downtrend.

## 🎛️ Customizable Inputs

You can easily adjust these settings via the indicator's settings panel on TradingView:

| Input Name | Default Value | Description |
| :--- | :--- | :--- |
| `Trend SMA Length` | `50` | Number of bars used to calculate the trend direction. |
| `RSI Length` | `14` | Lookback period for the RSI calculation. |
| `RSI Overbought Level` | `70` | Upper limit indicating temporary overbought conditions. |
| `RSI Oversold Level` | `30` | Lower limit indicating temporary oversold conditions. |
| `Show Background Highlights`| `true` | Toggles the translucent background green/red zones. |
| `Show Buy/Sell Markers` | `true` | Toggles the visual chart shapes and text. |

## 💻 How to Install and Use

1. Open your chart on **TradingView**.
2. Click on the **Pine Editor** tab at the bottom of the screen.
3. Delete any default code and paste the code from your `.pine` file.
4. Click **Save** and then click **Add to chart**.

## 📝 Specifications

- **Language:** Pine Script v6 (`//@version=6`)
- **Overlay:** `true` (Plots directly on the price chart)
- **Compatibility:** Works on all timeframes and assets (Stocks, Crypto, Forex, Indices).

## ⚠️ Disclaimer

This script is for educational purposes only. It does not constitute financial advice. Always combine technical indicators with proper risk management and your own trading plan.
