# Trading View Pine Script for the BTFDBot Super Oversold Swing Trading Strategy

Check [my YouTube Channel](https://www.youtube.com/@simpleswingtrading/) if you want to find out how this works, plus general other algotrading/swing-trading/quant stuff. This trading strategy works on stocks, ETFs, crypto, indexes and just about everything.

This is for backtesting in TradingView. If you need to know how to use the script then Google how to add a Pine Script custom indicator to a chart. It's NOT a scanner/screener. If you want to screen for stocks that are currently Super Oversold your options are:

1. [BTFDBot.com](https://www.btfdbot.com/): This is my backtester/trading signals site. It's free but only has the higher quality US stocks listed. I also post UK stocks on my socials. On BTFDBot this signal is called Super-Duper Oversold.
2. [FinViz](https://finviz.com/?affilId=717656427): Affiliate link but it's really appreciated if you support my work by using this link. You can only search for this signal using an Elite account - they don't allow scanning for a custom % above or below 52 week lows on a free account. Note that they also allow you to screen on 50 day lows. This can work well with good quality stocks.
3. Schwab's ThinkOrSwim but I haven't yet figured out how to code it in ThinkScript. Please do have a go at it if you're a ThinkScript genius.

Let me know if you find any other platforms that will allow screening for this setup. You basically need to screen for 52 week lows, and then the stock must drop 20% below the 52 week low in a certain timeframe (1 year max seems best).

This Pine Script backtests the BTFDBot Super Oversold trading strategy. This is a rare signal but has an extremely high win rate. Here's an example of it generating profits from Barclays (BARC) in the 2008 financial crisis. No losses even though the stock's largest drawdown from the 2007 peak was something crazy like 92%.

![Example of the Super Oversold Pine Script Backtested on Barclays (BARC) during 2008 - 2012](https://github.com/nichelaboratory/PineScript_SuperOversold/blob/main/Super-Oversold-Barc-2008.png)

Here's the same stock but a very long term backtest showing that this signal has NEVER not returned 10%:

![Example of the Super Oversold Pine Script Backtested on Barclays (BARC) in BTFDBot](https://github.com/nichelaboratory/PineScript_SuperOversold/blob/main/Super-Oversold-Barc-BTFDBot-Chart.png)

Again it's a rare signal but has an extremely high win rate (100% on many instruments).

There are various settings you can change in TradingView:

![Example of the Super Oversold Pine Script Backtested on Barclays (BARC) during 2008 - 2012](https://github.com/nichelaboratory/PineScript_SuperOversold/blob/main/Super-Oversold-Options.png)

Good backtesting stocks for this script: OLN, ARE, CE, SHOO, KSS
Long term backtesting (including the 2008 GFC): Barclays (BARC) 1990+ Land Securities (LAND) 1990+
Settings: just play around with them but be wary of curve fitting. With ETFs/super high quality stocks a 52 week low followed by a 5-7% drop may work better. You will get more signals but this will reduce the win rate.

On the Trading View chart:

Blue line: 52 week low Red line: Current Super Oversold price target
Blue down arrow: new 52 week low Red down arrow: Buy Pink down arrow: profitable exit from position
