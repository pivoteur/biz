# "I'm Not Selling!"

## Pivot Arbitrage vs. well: everything else

Is "I'm Not Selling!" a good strategy?

Well, yes and no.

Let's defend the HODL-strategy (or the "I'm not selling!"-strategy).

I looked at $BTC back in November of 2013 when it was $200-per. WAY overpriced, obviously. But what if I had bought 5 $BTC back then and never sold?

![$BTC at $200-per in November, 2013](imgs/arb/01-btc.png)

For my $1,000 investment, my assets today would be worth $505,000.

That's a Return on Investment (ROI) of 50,000%, annualized to 4,200%.

That's not bad in anyone's book, I'd say.

But remember the Bitcoin-proverb:

> 1 $BTC is 1 $BTC.

At the end of the day, I started with 5 $BTC, and I ended up with 5 $BTC.

Can I do better than that? Or, 5 $BTC is the baseline.

Pivot arbitrage addresses that question.

But, first of all, what is pivot arbitrage?

## Pivot Arbitrage

### The Ratio for a BUY or SELL signal

Pivot Arbitrage is the investment tactic that pits, or pivots, one asset, say $BTC, against another, say $USDC (the USD-stable token) (sometimes).

What pivot arbitrage does is pits one asset against the other. When BTC/USDC-ratio is 'low' that indicates the price of $BTC is low, relative to $USDC, so we buy $BTC and sell $USDC. Conversely, when the BTC/USDC-ratio is 'high,' that shows that $BTC-price is high (relative to $USDC) and $USDC price is low, so we buy $USDC and sell $BTC.

![BTC/USDC-ratio](imgs/arb/02a-ratio.png)

### The Delta for how much to buy or to sell

So we have our BUY or SELL signal.

Now, how confident are we in that signal?

The difference between the ratio and the EMA-20 (Exponential Moving Average of
the ratio over a 20-day period) – or simply, the δ ('Delta') – gives a measure
of confidence in that call. The larger the δ, the more confident in the call I
am.

I have a working understanding of confidence in that I have two classes based 
upon the magnitude of the δ. δs below 20% I classify as 'meh,' meaning that the
call is too close to call, either way. δs above 20% I classify as strong support
for the BUY or SELL signal.

![δ: a measure of confidence](imgs/arb/02b-delta.png)

This measure of confidence gives me the, well: confidence to execute the trades
to open pivots and hedges boldly (in the case of a strong δ) or timidly.

## Hedges

I mentioned "hedges" in the last section.

I employ hedging against my own strategy, because the Markets have been 
consistent in throwing curveballs against any strategy tried against them. This 
strategy has been working well in both Bear and Bull markets, and then I put the
pivoted assets into yield-bearing money markets, so when the markets are flat, 
I'm earning interest against the assets.
