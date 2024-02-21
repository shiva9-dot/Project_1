# STOCKSIFT Walkthrough

**STOCKSIFT**, is a market denoiser that allows early-stage investors a little peace of mind when making purchase decisions.
In the repository, there are five main focal points:
1. **The Resources Folder**: Important files and datasets that make it all run.
2. **Final Visualization Notebook**: A user-friendly visualizer that pulls data from the other notebooks.
3. **Risk_Evaluation Notebook**: Evaluate the risk of stocks on the market by beta, Value At Risk, volatility, and cumulative return—results in a list of 10 stocks based on user preferences.
4. **Long-term Analysis Notebook**: Takes the list of 10 stocks by the risk evaluator and generates an analysis of their long-term health and viability.
5. **Short-term Analysis Notebook**: Takes the list of 10 stocks by the risk evaluator and generates an analysis of their short-term health and viability.
6. Two zipfiles containing stock datasets

## Presentation
- Check out a presentation link for more context: [STOCKSIFT Presentation](https://www.canva.com/design/DAFxeHRpI5c/hGyI2nRsmO2C-EnDP72z9Q/view?utm_content=DAFxeHRpI5c&utm_campaign=designshare&utm_medium=link&utm_source=editor).

## Datasets
- **SP500 Data** was imported from `yfinance`. All other datasets are in the Resources folder.
- **'World Stock Prices Dataset'** and **'World-Stock-Prices-Dataset'** both originated from the global daily stock dataset from Kaggle. It can be found here: [World Stock Prices (Daily Updating)](https://www.kaggle.com).
- The `bond_yields` dataset was downloaded as a comparison set for the Risk Analysis. Comparing the risk level of different stocks to the safety of government bonds and finding the difference in bond risk ratios.
- All other datasets were generated CSVs that saved specific data for export.

## Final Visualization
- **Guarantee Directory** - You’ll need to plot to the Project directory here. We had to hard code it because of Jupyter lab preferences for running each other's code.
- Restart the Kernel, and you can fiddle with the inputs. Your first two options are 'current' and 'history' for short-term and long-term breakdowns, respectively. The next input is the term over which your risk will be calculated, options being 7Dys, 21Dys, 40Dys, 1Yrs, 5Yrs, 10Yrs, 15Yrs. The last input is if you want a list of stocks that are high risk, low risk, or average risk; the options are high, low, and mid.

## Risk Evaluation
- Ensure the 'World_Stocks' and 'Bond_yields' variables are mapped to the right CSVs in the Project_Uno folder.
- The final output should be a list of 10 stocks based on user preferences, the Beta and Volatility values for those 10 stocks, and the original stock data for those 10 stocks.

## Long-Term Analysis
- The long-term analysis provides data for SMA, Sharpe Ratios, Volume, and Annualized/Cumulative Returns for the 10 stocks selected in the risk evaluation.

## Short-Term Analysis
- The short-term analysis provides data for MACD, RSI, Moving Average, and Daily Return for the 10 stocks selected in the risk evaluation.
