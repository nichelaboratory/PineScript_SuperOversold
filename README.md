# Trading View Pine Script for the BTFDBot Super Oversold Swing Trading Strategy

Check [my YouTube Channel](https://www.youtube.com/@simpleswingtrading/)) if you want to find out how this works, plus general other algotrading/swing-trading/quant stuff.

This is for backtesting in TradingView. If you need to know how to use the script then Google how to add a Pine Script custom indicator to a chart. It's NOT a scanner/screener. If you want to screen for stocks that are currently Super Oversold your options are:

1. [BTFDBot.com](https://www.btfdbot.com/): This is my backtester/trading signals site. It's free but only has the higher quality US stocks listed. I also post UK stocks on my socials.
2. [FinViz](https://finviz.com/?affilId=717656427)): Affiliate link but it's really appreciated if you support my work by using this link. You can only search for this signal using an Elite account - they don't allow custom % above or below 52 week lows on a free account. Note that they also allow you to screen on 50 day lows. This can work well with good quality stocks.
3. ThinkOrSwim but I haven't yet figured out how to code it in ThinkScript.

Let me know if you find any other platforms that will allow this. You basically need to screen for 52 week lows, and then the stock must be X% below the 52 week low.

This Pine Script backtests the BTFDBot Super Oversold trading strategy. This is a rare signal but has an extremely high win rate. Here's an example of it generating profits from Barclays (BARC) in the 2008 financial crisis. No losses even though the stock's largest drawdown from the 2007 peak was something crazy like 92%.

![Example of the Super Oversold Pine Script Backtested on Barclays (BARC) during 2008 - 2012](https://github.com/nichelaboratory/PineScript_SuperOversold/blob/main/Super-Oversold-Barc-2008.png)

There are various settings you can change in TradingView:

![Example of the Super Oversold Pine Script Backtested on Barclays (BARC) during 2008 - 2012](https://github.com/nichelaboratory/PineScript_SuperOversold/blob/main/Super-Oversold-Options.png)
