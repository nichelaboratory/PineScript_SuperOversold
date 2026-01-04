# Trading View Pine Script for the BTFDBot Super Oversold Swing Trading Strategy

Super Oversold is a trading strategy with an exceedingly high win rate (100% on most quality stocks). What we're looking for is a stock to make a 52 week low and then drop another 20%. This is an extremely rare setup but when it happens the chances of the stock bouncing are incredibly high. We aim to capture a quick 5-10% swing trade off the Super Oversold buy signal.

The strategy does not use stop losses. Instead we hodl for 1 year and if it doesn't sell then we adjust the sell price to the buy price in an attempt to break even. If it doesn't sell after another year we sell the stock.

The strategy works on anything (stocks, ETFs, crypto etc.) but be wary of using it on penny stocks. Also be wary of using it on anything coming off of an obvious bubble. For lower risk assets you will have to reduce the Super Oversold Target % option to 5-7% or something but be wary of curve fitting.

Check [my YouTube Channel](https://www.youtube.com/@simpleswingtrading/) if you want to find out how/why this works, plus general other algotrading/swing-trading/quant stuff. This trading strategy works on stocks, ETFs, crypto, indexes and just about everything.

This script is for backtesting in TradingView. If you need to know how to use the script then Google how to add a Pine Script custom indicator to a chart. It's NOT a scanner/screener. If you want to screen for stocks that are currently Super Oversold your options are:

1. [BTFDBot.com](https://www.btfdbot.com/): This is my backtester/trading signals site. It's free but only has the higher quality US stocks listed. I also post UK stocks on my socials (my Substack is [here](https://simpleswingtrading.substack.com/). On BTFDBot this signal is called Super-Duper Oversold. The original Super Oversold strategy on the site works off of other initial signals. But after analysing over 1000 stocks I found Super Oversold works best from 52 week lows. So that is what I coded into this Pine Script.
2. [FinViz](https://finviz.com/?affilId=717656427): Affiliate link but it's really appreciated if you support my work by using this link. You can only search for this signal using an Elite account - they don't allow scanning for a custom % above or below 52 week lows on a free account. Note that they also allow you to screen on 50 day lows. This can work well with good quality stocks.
3. Schwab's ThinkOrSwim but I haven't yet figured out how to code it in ThinkScript. Please do have a go at it if you're a ThinkScript genius.

Let me know if you find any other platforms that will allow screening for this setup. You basically need to screen for 52 week lows, and then the stock must drop 20% below the 52 week low in a certain timeframe (1 year max seems best).

Super Oversold is a rare signal but has an extremely high win rate. Here's an example of it generating profits from Barclays (BARC) in the 2008 financial crisis. No losses even though the stock's largest drawdown from the 2007 peak was something crazy like 92%.

![Example of the Super Oversold Pine Script Backtested on Barclays (BARC) during 2008 - 2012](https://github.com/nichelaboratory/PineScript_SuperOversold/blob/main/Super-Oversold-Barc-2008.png)

Here's the same stock but a very long term backtest showing that this signal has NEVER not returned 10%:

![Example of the Super Oversold Pine Script Backtested on Barclays (BARC) in BTFDBot](https://github.com/nichelaboratory/PineScript_SuperOversold/blob/main/Super-Oversold-Barc-BTFDBot-Chart.png)

Again it's a rare signal but has an extremely high win rate (100% on many instruments). Here's Steve Madden (SHOO):

![Steve Madden SHOO Super Oversold Trading View Backtest Results](https://github.com/nichelaboratory/PineScript_SuperOversold/blob/main/Super-Oversold-Steve-Madden-SHOO.png)

While we didn't beat buy and hold, over the lifetime of this stock we made 62.12% and the average time in trade was just 28 days (145.9% CAGR).

There are various settings you can change in TradingView:

![Example of the Super Oversold Pine Script Backtested on Barclays (BARC) during 2008 - 2012](https://github.com/nichelaboratory/PineScript_SuperOversold/blob/main/Super-Oversold-Options.png)

Good backtesting stocks for this script: OLN, ARE, CE, SHOO, KSS

Long term backtesting (including the 2008 GFC): Barclays (BARC) 1990+ Land Securities (LAND) 1990+

Settings: just play around with them but be wary of curve fitting. With ETFs/super high quality stocks a 52 week low followed by a 5-7% drop may work better. You will get more signals but this will reduce the win rate.

On the Trading View chart:

Blue line: Level of the previous 52 week low
Red line: Current Super Oversold price target
Blue down arrow: new 52 week low
Red down arrow: Buy
Pink down arrow: profitable exit from position
