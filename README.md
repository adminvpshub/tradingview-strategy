# TradingView Strategy Template

This repository contains a Pine Script v5 strategy for TradingView. It implements a simple Moving Average Crossover strategy as a starting point, which you can easily customize.

## Features

- **Backtesting Ready**: Uses `strategy()` functions to allow backtesting in the Strategy Tester.
- **Visual Signals**: Displays "BUY" and "SELL" labels directly on the chart.
- **Configurable**: Fast and Slow MA lengths can be adjusted in the settings.

## How to Use

1.  **Open TradingView**: Go to [tradingview.com](https://www.tradingview.com/chart/).
2.  **Open Pine Editor**: At the bottom of the chart interface, click on "Pine Editor".
3.  **Copy Code**: Copy the contents of `strategy.pine` from this repository.
4.  **Paste Code**: Delete any existing code in the Pine Editor and paste the code you just copied.
5.  **Save**: Click "Save" and give your script a name (e.g., "My Custom Strategy").
6.  **Add to Chart**: Click "Add to chart". You should see the Moving Averages and Buy/Sell labels appear.
7.  **Backtest**: Click on the "Strategy Tester" tab at the bottom to see how the strategy performed on historical data.

## How to Publish to GitHub

Since this code was generated locally, you can push it to your own GitHub account by following these steps:

1.  **Create a Repo**: Go to [github.com/new](https://github.com/new) and create a new empty repository (do not initialize with README/gitignore).
2.  **Push Code**: Run the following commands in your terminal (inside this `tradingview-strategy` folder):

```bash
# Initialize git if you haven't already (already done in this setup)
# git init
# git add .
# git commit -m "Initial commit"

# specific commands to push:
git branch -M main
git remote add origin https://github.com/<YOUR_USERNAME>/<YOUR_REPO_NAME>.git
git push -u origin main
```

## Customization

To change the logic, edit the `strategy.pine` file. Look for the `// Trading Logic` section:

```pinescript
// Example: Change to RSI
// rsiValue = ta.rsi(close, 14)
// longCondition = ta.crossover(rsiValue, 30)
// shortCondition = ta.crossunder(rsiValue, 70)
```
