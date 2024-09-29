# Pivot Technologies, LLC.

Welcome.

1. What is pivot arbitrage? How does it differ from traditional arbitrage and
from liquidity pools (LPs)?
2. What is the pivot protocol ecosystem?
3. How do I do this thing?

## Pivot arbitrage

### First, what is traditional arbitrage?

Okay. First things first. Pivot arbitrage is not like traditional arbitrage
in its operation.

In traditional arbitrage, you trade $25k of $ETH by buying on one DEX or CEX
and selling on another all in the same transaction. 1% profit would be $250,
but traditional arbitrage seldom, if ever, reaches the 'heights' of 1% ROI.
0.10% to 0.25% ROI is the normal anticipated gain, which translates into
you risking $25k of $ETH for a possible $25 - $50 gain.

If the arbitrage goes wrong, you lose some, or all, of your $25k $ETH.

That's why there are contracts to do the entire buy-sell trades, across DEXen,
as one transaction, and they have bots to do this for you, so you can do
100s of these per day.

So: if the bot goes haywire, ... so, too, does your principal, as well.

Very ... 'fun.' Very exciting. Very, very, paltry returns.

People make a lot of money by handcuffing themselves to their keyboards in
this way.

If this is you, more power to you.

This, traditional arbitrage, is not me, however.

### What is pivot arbitrage?

Pivot arbitrage, on the other hand, is based upon this conceit: coins of value,
let's say $BTC and $ETH for this example, go up and go down, and, as coins of
value, they _do_ go back up after going down, and: they aren't up-only, either,
they come back down.

Now, most of the cryptouniverse of tokens are highly volatile, and also highly
in synch with $BTC's volatility. $BTC goes up, all of crypto go up. $BTC goes
down, all of crypto goes down ... hard, in fact.

But here's the thing: the cryptocurrency market is not efficient. There are
variabilities, token-to-token.

So, sticking with the BTC/ETH example, BTC goes up, ETH goes up. BTC goes down,
ETH goes down, but, observe this: not at the exact same time, sometimes, not
even close.

The _ratio_ of BTC/ETH is the blue line on the chart here.

![BTC/ETH ratio](imgs/01-btc-eth-ratio.png)

Notice in the above ratio (the blue line) there are peaks and valleys.

* on the peaks, $BTC's price is high, relative to $ETH, so you swap $BTC to
$ETH
* on the valleys, $BTC's price is low, relative to $ETH, so you swap $ETH to
$BTC

A _pivot_ *has* a principal asset, say, for example, $BTC, and a pivot asset,
which would be $ETH in this case.

A _pivot_ *is* two trades, the opening trade (say on 2024-06-28), where we 
trade the principal asset ($BTC, in this case) for $ETH, and the closing 
trade (say on 2024-08-09), where we trade the exact same amount of $ETH for 
$BTC.

More $BTC.

... much more $BTC.

As you recall, traditional arbitrage expects gains of 0.10% to 0.25% ROI.

Pivot arbitrage, on the other hand, sees gains between 10% to 40% ROI.

Let's prove this out – shall we? – by using the example from above. We're going
to walk through 2 pivots, one on $ETH as the principal asset, and one on $BTC
as the principal asset. We'll do the pivots using my technology, unexplained
for now, show that it works, and how it works via the opening and closing
pivot trades, then explain what's going on, mathematically, as we develop
the technologies used, in this whitepaper.

On y va.

### Scenario: Pivot arbitrage on 1 $BTC and 18.5 $ETH starting 2024-03-04

1. On 2024-03-07, open an $ETH-pivot by swapping 1.36 $ETH for 0.08 $BTC. 
Why? Because the BTC/ETH ratio is _below_ the EMA-20-line, indicating that 
$BTC is 'cheap,' ... relative to $ETH, that is.

![Open ETH pivot](imgs/02a-open-eth-pivot.png)

2. On 2024-03-19, close the $ETH-pivot by swapping the 0.08 $BTC back, but now
we get 1.53 $ETH.

![Close ETH pivot](imgs/02b-close-eth-pivot.png)

So, with a swap, then, later, a swap back, we've made 0.17 $ETH.

From 1 $BTC and 18.5 $ETH on 2024-03-04, we now have 1 $BTC and 18.67 $ETH on
2024-03-19.

Now, let's do a $BTC-pivot.

1. On 2024-04-13, we open a $BTC-pivot by swapping 0.09 $BTC for 1.87 $ETH.

![Open BTC pivot](imgs/02c-open-btc-pivot.png)

2. On 2024-04-29, we close the $BTC-pivot by swapping back the 1.87 $ETH, but
for 0.094 $BTC now.

![Close BTC pivot](imgs/02d-close-btc-pivot.png)

After two pivots, our initial positions of 1 $BTC and 18.5 $ETH are now 1.094
$BTC and 18.67 $ETH.

That is to say, by using pivot-arbitrage, we have grown _both_ our $BTC and
$ETH positions, _monotonically increasing, safely_ both sides of the 
pivot-pool.

### Pivot arbitrage vs Liquidity Pools (LPs)

We've covered how pivot arbitrage is fundamentally different from traditional
arbitrage, both in practice and in pacing. How, then, does pivot arbitrage
differ from supplying liquidity to LPs? After all, you're supplying both
$BTC and $ETH liquidity to the pivot arbitrage pool, just like you supply
the same liquidity to the ETH/BTC LP.

* Liquidity Pools

Liquidity pools serve a very useful function in the cryptocurrency ecosystem,
particularly for DEXen. You, the j-random investor, provide liquidity, and
the DEX uses to keep prices fair for swaps. If I'm trading $ETH for $BTC, the
DEX goes to the ETH/BTC LP and pulls the $BTC from those reserves for the
$ETH you provide to swap.

The deeper and stronger a liquidity pool, the easier swaps occur on these
exchanges.

So: Liquidity Pools Я good, ... for these exchanges, anyway.

Are they good for you?

Not really, if we're being honest (and honesty in trade makes everything better
for everybody), and that's why DEXen provide incentives for you to provide
liquidity. The incentive: "You provide tokens popular in swaps and we'll 
reward you with our protocol tokens."

Now, how do the protocol tokens do over time? If they don't have an intrinsic
value (and 'providing incentive' is not an intrisic value for a token), then
these tokens, sooner or later, fall to their real value, ... and usually
sooner if they're being printed to provide incentives.

That's one issue with LPs: they usually have artifical incentives to invest
into them.

The other problem for you, the investor, into LPs, is their very structure:

> xy = k

LPs, as automated by market makers (AMMs), usually are offerd as xy = k.

What does this formula mean?

It means if you provide liquidity to the ETH/BTC LP, you're providing
$ETH (x) and $BTC (y) to the pool (k).

So as the number of tokens of $ETH go up, what happens to your $BTC?

If the pool is constant (which 'k' means: 'konstant,' because we're German,
now, for some reason), it means your $BTC-count goes down.

Vice versa applies, as well, as $BTC-count goes up, $ETH-count goes down.

But that's the nature of investing in LPs, isn't it?

Sure it is, but that doesn't mean that's the only game in town. This is your
money, after all, right? Why not play a better game?

"What better game?" you ask.

Glad you asked.

* Pivot pools

An alternatives to liquidity pools that we offer is the pivot pool. Unlike
the xy = k formulation of how liquidity pools operate, pivot pools have the
following formulation:

> x<sub>t</sub> + y<sub>t</sub> = P<sub>t</sub>

What does this formulation mean? and how does it differ from how Liquidity
pools work?

What this formulation means is that when you provide $ETH (x<sub>0</sub>) and 
$BTC (y<sub>0</sub>) to the pivot pool (P<sub>0</sub>) there are two significant
differences from how liquidity pools operate. The first, and most obvious,
difference is that the $ETH and $BTC provided are _additive_ to the pivot
pool, not _multiplicative_ as they are in the Liquidity pool. This means for
you, the investor that as the pivot pool grows over time (from P<sub>0</sub> to
P<sub>1</sub> to P<sub>2</sub> and so on), _either_ your $ETH is growing _or_
your $BTC is growing, independent of each other, _or both_ are growing as the
pivot pool grows.

That's a significant difference from liquidity pools.

* In liquidity pools, x and y are _dependent_ variables where one asset's growth
inversely affects the other asset.
* In pivot pools, x and y are _independent_ so the growth of one does not
inversely impact the growth of the other asset at all, and, in fact, both
can be growing at the same time if pivot-positions are open for both assets
at the same time.

Investing into liquidity pools is very definitely a valid strategy and used
to great success by investors who have a clear aim with this instrument.

But.

But, by investing in an xy = k LP, you are, in effect, betting one asset
against the other in the LP. If both assets are assets of value and you want
to see the growth of both, LPs are not the most effective, and, in fact, are
always less efficient than if you simply hold both assets separately. It is
better for both assets for you to invest into the pivot protocol.

So, that is also why it's necessary for pivot pools only to have assets of
value in their pools. The success of these pools depend upon this.

How so?

If you have a pivot pool with, say, $LUNA (in the original Terra) and say, 
$PSI, which turned out to be a down-only asset, then the EMA-20 curve will 
show $LUNA is 'overpriced' as compared to $PSI. All the $LUNA eventually is 
drained to the down-only $PSI: you're left with all $PSI in a downward spiral 
as $LUNA rose from $5 to $120.

How do I know this? Because LPs have the same weakness: as $LUNA rose in
price, the LP rebalanced to less $LUNA to more $PSI. All my $LUNA was drained
to $PSI which, even with '1,500% APY' $PSI yields, became worthless against
the $LUNA originally invested into the LP.

Pivot pools protect against this by pivoting on assets of like- or 
similar-value. Therefore you have an $ETH+$BTC pivot pool. Why? Because both
$ETH and $BTC go up and down, but they have a history of recovering from
crashes multiple times: they've proved their resiliency.

