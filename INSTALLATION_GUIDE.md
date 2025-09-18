# Pine Script Installation Guide

## Quick Installation Steps

### 1. Copy the Pine Script Code
- Open the file `advanced_sr_indicator.pine` in this repository
- Copy all the code (Ctrl+A, Ctrl+C)

### 2. Open TradingView Pine Editor
- Go to TradingView.com
- Open any chart
- Press **Alt + E** or click the "Pine Editor" tab at the bottom

### 3. Paste and Add to Chart
- Clear the editor if there's existing code
- Paste the copied code (Ctrl+V)
- Click "**Add to Chart**" button

### 4. Configure Settings (Optional)
- Click the gear icon ⚙️ next to the indicator name
- Adjust settings according to your preferences:
  - **S/R Lookback Period**: 20 (default)
  - **S/R Sensitivity**: 0.5 (default, lower = more levels)
  - **Enable patterns**: Doji, Harami, Engulfing
  - **Enable alerts**: BUY/SELL signals

### 5. Set Up Alerts (Optional)
- Right-click on the chart
- Select "Add Alert"
- Choose your indicator from the dropdown
- Configure alert conditions

## Default Settings Explanation

| Setting | Default | Description |
|---------|---------|-------------|
| S/R Lookback | 20 | Number of bars to look back for pivot points |
| S/R Sensitivity | 0.5 | Lower = more sensitive (more S/R levels) |
| S/R Timeframe | Current | Timeframe for S/R calculation |
| Max S/R Levels | 10 | Maximum number of S/R levels to display |
| Max Labels | 20 | Maximum number of signal labels on chart |

## Performance Tips

**For better performance:**
- Increase S/R Sensitivity (0.7-1.0) for fewer levels
- Reduce Max S/R Levels (5-8)
- Use higher timeframes for S/R calculation

**For more accuracy:**
- Decrease S/R Sensitivity (0.2-0.4) for more levels
- Increase lookback period (30-50)
- Use current timeframe for S/R calculation

## Troubleshooting

**Error: "Script could not be translated"**
- Make sure you copied the complete code
- Check for any missing characters
- Try refreshing the Pine Editor

**Too many S/R levels displayed**
- Increase S/R Sensitivity value
- Reduce Max S/R Levels setting

**No signals appearing**
- Check if patterns are enabled in settings
- Verify that alerts are enabled
- Ensure you're on a timeframe with enough data

## Features Overview

### 📈 Support/Resistance Zones
- Automatically detects key price levels
- Visual representation with boxes or lines
- Configurable sensitivity and timeframe

### 🕯️ Candlestick Patterns
- **Doji**: Indecision candles
- **Harami**: Inside bar patterns (bullish/bearish)
- **Engulfing**: Complete engulfment patterns

### 🔔 Alerts
- BUY signals near support with bullish patterns
- SELL signals near resistance with bearish patterns
- Customizable alert frequency

### 📊 Statistics Table
- Real-time signal counts
- Estimated win-rate
- Active S/R levels count

Happy trading! 📈