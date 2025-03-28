#  Pivot Technologies, LLC.

## Pivot Protocol whitepaper

[HWÆT](https://blogs.bl.uk/digitisedmanuscripts/2013/02/beowulf-online.html)

![HWÆT](imgs/00-HWÆT.jpg)

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

## Pivot protocol ecosystem

### Components

![pivot protocol components](imgs/components/01-components.png)

The pivot protocol is composed of the following components:

1. The pivot pools
2. The echo pools
3. The treasury
4. Measuring performance / Calculating apportionment
5. The you, the investor
6. Investing liquidity

We well go over each component in turn.

### 1. The Pivot Pools

![The BTC+ETH pivot pool](imgs/components/01a-pivot-pool.png)

The pivot pools repose the pivot asset and the principal asset (shown here is
the BTC+ETH pivot pool). Here is where the magic happens, that is to say: where
opening and closing pivot transactions occur with the pivot and principal
assets, growing one, the other, or both assets.

The only way the investor (the you) can invest into any part of the protocol
is to use the protocol asset, which, for the pivot protocol is the 
[$UNDEAD token](https://www.undeadblocks.com/token-address), 

![The $UNDEAD token](imgs/components/currency/undead.png)

... which is due in thanks to a generous grant from 
[Wagyu games](https://www.wagyu.io/).

The pivot pools pay-out pivot arbitrage-gains to the investor (the you), its 
corresponding echo pool, to the treasury, and back to itself.

With each pivot, the pivot pool grows the protocol. All of it.

Each pivot pool is incubated with 50% of its total market capitalization from
investments of liquidity from both Wagyu Games and the Pivot Protocol.

### 2. The Echo Pools

![The BTC+ETH echo pool](imgs/components/01b-echo-pool.png)

While pivot arbitrage is occuring in the pivot pools (1., above), at the same
time, there is pivot arbitrage occuring focused on protocol-growth in the
echo pools (here we have the BTC+ETH echo pool, which also includes the protocol
token, $UNDEAD).

In the echo pool, pivot arbitrage occures between the pivot and principal assets
(as 1., above), but pivots are also occuring between the protocol asset and the
pivot and principal assets.

Why?

This not only increases the principal and pivot assets in the pool, but also
increases the protocol asset.

As the protocol asset is the only way to invest into protocol, even for 
investments from the protocol, itself, the echo pool serves to grow the 
protocol's depth and strength by growing the protocol asset via pivot arbitrage.

The echo pools pay out to the investor (the you) and to the treasury.

Each echo pool is funded with 50% of its market capitalization from liquidity
provided by Wagyu Games and the Pivot Protocol.

### 3. The Treasury ([_Norge_](https://en.wikipedia.org/wiki/Norway))

![The Treasury](imgs/components/01c1-treasury-norge.png)

The treasury is the 'safe zone' for assets created and invested into the
protocol. No trading activity occurs in the treasury, but, instead, the
investor (the you) may invest into the treasury to receive pay-outs from the
treasury in two ways:

1. For each gain received from the pivot pools (1.) and echo pools (2.), a
percentage is paid-out to the investors.
2. Like for Norway's Oil Fund (officially named the
[Government Pension Fund of Norway](https://en.wikipedia.org/wiki/Government_Pension_Fund_of_Norway)),
a small annual percentage of the treasury is disbursed to investors.

The aim of the treasury, like the Norway Oil Fund, is to grow so large that
this 'small annual percentage disbursement' grows to be quite large over time,
and this is effected in two ways.

1. The small annual percentage disbursement, so that the liquidity grows large
without interruption from sticky fingers of people who want money now.
2. Investments into promising opportunities, both 
* _internally_ into new pivot pools, renewed pivot pools (like, say, if BTC+ETH 
becomes so popular that it hits its market cap and there is demand for more of 
the same), and new kinds of pivot, or other kinds of, pools, as technology 
develops; and,
* _externally_ if a bright-eyed, promising, energetic founder has the next 
killer idea (with a year's worth of transactions as a track-record to prove 
their pitch).

The latter will occur only under two conditions,.

1. A maximum of 10% of treasury funds is to be used for ventures at any time.
2. So that means that the treasury has to be large enough at the point for
investment opportunities to be considered.

Just as Wagyu Games saw an opportunity in the pivot protocol to make an
investment, incubating this protocol, the pivot protocol may invest into
promising new developments that push advancements in cryptocurrency and its use.

The treasury is initially funded by liquidity from both Wagyu Games and the
Pivot Protocol.

### 4. Asset apportionment / Measuring performance of pivot arbitrage

#### The problem, or: why 'just doing math' is problematic.

How do we know pivot arbitrage works?

Measure, of course.

Measure what? That we have more tokens? Yes, again: of course.

But when pivot arbitrage relies on at least two tokens, of *very* different
characteristics (price, say), then measuring the performance becomes more 
tricky than it appears at face value.

What do I mean by this? Let's construct a thought-experiment. Say you have a 
$BTC + $ETH pivot pool that starts out at $500,000. Some pivot arbitrage occurs
then the pivot pool is worth $600,000.

Was the pivot arbitrage successful? Sure! you say, but hold on there, pardner!

The price has gone up, and that's great, but was that due to the price-movement
of the individual tokens, or was that due to the pivot arbitrage?

Well, if $USD-value of the portfolio is not a measure of pivot arbitrage 
success (and, this is not a spoiler at all: it is not), then is number of
tokens the measure of success?

... no. I mean, not precisely. And let's do another thought experiment to
illustrate why.

Say you started your $500,000-portfolio with 4.1 $BTC and 104 $ETH. Then you
do some pivot arbitrage and now you have 5.2 $BTC and 110 $ETH, but the 
portfolio $USD value is now $485,000. Was pivot arbitrage successful?

Yes. Yes, it was.

HOW successful was it, *exactly?* And, by *exactly,* I mean what is each
pivot's ROI? ... what is each pivot's APR? ... what is the pool's APR? What
was the original apportionment of $BTC in the pivot pool? (Hint: it was 50%)
What was the original apportionment of $ETH in the pivot pool? (Same hint)

But the trickier question is: what is the apportionment of $BTC and $ETH in the
current pool, and what percentage gain of each asset occured from the original
pivot pool?

Now you can do math and get the answers to the above questions, but that 
requires you have the context of what the $BTC and $ETH prices *were* to compute
their original apportionment (of course), but also to compare the the results
you have, pivot to pivot, to get to the pools current value and apportionment.

#### The Solution: γ-factor

I do have experience in this domain. Originally, I had tracked the success
of pivot arbitrage by starting with a set-amount of the assets, and then,
when one of the assets returned to the started amount, did I have more of the
other? (Yes, I did) And when the *other* asset resettled to the starting amount
did I have more of the first? (Yes, I did) And when I had more of both, I used
that as a locus to restart my measures, proving pivot arbitrage went from more
to even more of the pivoted assets.

That's great, and that's reassuring, ... but it's not precise.

What this approach *did* give me, even though it *didn't* give me precision, was
that it *did* give me the insight that I needed to calculate 
token-apportionment, independent of price, and a way that, say, $BTC's growth
could be compared, apples-to-apples, to say, $ETH's growth.

Enter the γ-factor.

#### What is the γ-factor?

The γ-factor is different for each token *in* each pivot pool. That is to say:

* γBTC differs from γETH, but also 
* γBTC in the BTC+ETH pivot pool differs from γBTC in the BTC+PAXG+BNB pool.

Or: the γBTC-factor value applies *only* to the pivot pool for which it was
calculated, so, in fact, I could write γBTC<sub>ETH</sub> for the γBTC factor
value in the BTC+ETH pivot pool and γBTC<sub>PAXG+BNB</sub> for the
BTC+PAXG+BNB pivot pool, but I prefer the brevity of γBTC and allow the pivot
pool for which it is being used to provide that context.

But, still: what is the γ-factor, or, more precisely, how is it used?

The γ-factor of a token is a factor applied to the token-amount to provide
the apportionment of that token in the pivot pool.

> #btc tokens * γBTC-factor = γBTC

Or: 

> "The number of $BTC tokens multiplied by the γBTC-factor is the $BTC
apportionment of the pivot pool."

What is the 'token-apportionments' in a pool?

Again, a simple-sounding question that actually has a rather complex answer.

The token-apportionments sum to 100.0 on the incept of a pivot pool, but 
thereafter the token-apportionments change. Its value can go up or down, due 
to pivot arbitrage, but after all open pivots are closed, the token 
apportionments will be monotonically greater than the last time the pivot pool
had no open pivots.

#### Calculating the γ-factors of a pivot pool

Let's start with the incept of the BTC+PAXG+BNB pivot pool.

![BTC+PAXG+BNB pivot pool incept](blog/2024/10/09/imgs/03-paxg-pivot-pool-apportionment.png)

Here we see the γ-factors already calculated, so let's calculate them, 
step-by-step, and arrive at the solutions shown here.

1. At a pivot pool's incept, record the number of tokens for each token-type
and the token-prices.

2. Compute total $USD amount of each token and the total $USD value of the pool.
These are the `BTC $`, `PAXG $`, `BNB $`, and `Total $` amounts.

> e.g.: BTC $ = BTC (amount) * BTC quote

Do that for each token-type of the pivot pool.

3. From these values you can now compute the percentages of pivot pool for each
token.

> e.g.: BTC % = BTC $ / Total $

The token percentages should sum to 100%

4. Now that we have percentages using $USD, we can now compute the γ-factor

> γ-factor = token % / token amount * 100

This γ-factor, computed on pivot pool incept, is frozen. It's computed once
and that value is used thereafter as a constant.

5. The γ-apportionment of a token is now:

> e.g. γBTC = γBTC factor * BTC amount

As the γ-factor is frozen, but the number of tokens varies, we now have a way
to measure disparate tokens in a pivot pool uniformly, thus achieving our
apples-to-apples comparison for all tokens in the pivot pool.

![PAXG pivot pool after a trade](blog/2024/10/09/imgs/06-paxg-pivot-pool-after-trades.png)

### 5. The investor (the you)

![The Investor (the you)](imgs/components/01d-investor.png)

Hi, you! This is what makes the protocol work. 100% of the liquidity comes from 
the you, the investor.

How does this work?

## Investing into the Pivot Protocol

You, the investor, can invest your liquidity into the protocol in three ways:

1. Investing into the pivot pools
2. Investing into the echo pools
3. Investing into the treasury

Let's discuss each investment-approach in turn.

### Investing into the pivot pool

![Investing into pivot pools](imgs/investing/01-invest-pivot-pool.png)

Let's say you invest 10,000 $UNDEAD tokens into the BTC+ETH pivot pool (1.,
above). The pivot protocol takes that exact amount of $UNDEAD tokens, 10,000
tokens, – _not_ from the treasury, but from its own reserves – and swaps those 
tokens, over time, to the pivot and principal assets of the pivot pool (so, the
protocol would swap 10,000 $UNDEAD to $ETH and $BTC tokens) and deposit those 
tokens into the pool. Say you are the first and only investor during the first 
few pivots, you would then receive 100% of the gains allocated to investors 
into to the pool.

Those gains you receive as yields: are they $UNDEAD tokens, like the yields
are paid in protocol tokens, as they are for other protocols?

No, my dear investor. No, they are not.

The yields from your invested $UNDEAD liquidity are paid out in the pivot pool
gains. That means that the gains on a $BTC-pivot, say, are paid out in $BTC,

Not paid in $UNDEAD. $BTC gains are paid in $BTC.

Correspondingly, the gains on an $ETH-pivot are paid on your $UNDEAD investment
in $ETH.

Not paid in $UNDEAD. $ETH gains are paid in $ETH.

Let that sink in.

![Let that sink in](imgs/03-let-that-sink-in.jpg)

Cool.

### Investing into the echo pool

![Investing into the echo pool](imgs/investing/02-invest-echo-pool.png)

Investing into an echo pool is the same as investing into a pivot pool, as an
echo pool is a pivot pool.

However, the aim of the echo pool is quite different. The aim for the pivot
pool is to grow the principal and pivot assets. The aim, however, for the
echo pool is to grow the protocol asset, so this kind of pool must be deemed
as _high risk_ as the returns and value depend heavily upon the protocol
token's value.

That said: this is a good investment for you, the investor, if your aim is to
grow your protocol token bag.

As before, you, the investor, invest $UNDEAD liquidity into the echo pool. The
protocol takes an equal number of $UNDEAD tokens, placing (e.g.): $ETH, $BTC, 
and $UNDEAD tokens (using the BTC+ETH echo pool for this example). The Pivot
Protocol then executes pivot arbitrage with these tokens, and for yields you get
in return (less) principal assets, (less) pivot assets, and (more) protocol
assets.

### Investing into the Treasury

![Investing into the Treasury](imgs/investing/03-invest-treasury.png)

Like with investing into the pivot pools and echo pools, you, the investor,
invest $UNDEAD tokens into the treasury. As the treasury grows from profits 
from pivots occuring in the pivot pools and echo pools, it disburses a 
percentage of this growth to the investors.

It also disburses an annualized percentage of the treasury's entire value to
investors. 

So, for example, if the treasury is composed of, say:

* 156 $BTC
* 1560 $ETH and
* 1,560,000 $UNDEAD

and it disbursed weekly, the a disbursement, _in total to all investors_, would
be:

* 0.09 $BTC
* 0.9 $ETH and
* 900 $UNDEAD

And so, if you had invested $UNDEAD comprising 10% of the treasury's 
investments, for example, then you would receive:

* 0.009 $BTC
* 0.09 $ETH and
* 90 $UNDEAD

as your disbursment.

Since the Treasury receives a percentage of all pivot arbitrage profits, the
yields from the Treasury you would receive would be comprised of a percentage
of all pivot and echo pool profits.

However, it must be said that your returns on your investment into the Treasury
are lower than investments into any specific pivot or echo pool.

Also, investing into the treasury could be characterized as 'boring' by some
investors, as all the Treasury does is just sit there, receiving then disbursing
profit from the active pivot pools.

### Investment summary

You, as the investor, may invest in

* none of the above types
* one of the above types – pivot pools, echo pools, or the treasury
* some of the above types
* all of the above types of investment vehicles.

Your investment approach depends on your investment goals and tolerance to risk.

### 6. Investing liquidity

Let's look at how we translate invested liquidity into pivot assets. Recall our pivot pool and echo pool components. 

![Pivot Pools](imgs/components/01a-pivot-pool.png)
![Echo Pools](imgs/components/01b-echo-pool.png)

Is this an accurate representation of the pools? Yes, at the component-level, but there's more going on. Let's zoom into the components to get to the details of how the DCA-r, ./otto, works. 

Each pool is actually 3 wallets: 

![Pool wallets](imgs/components/02a-pool-wallets.png)

1. the investor stake, 
2. the pool, itself,
3. the reserve

Why? Let me explain. 

![Investment liquidity flow](imgs/components/02b-dca-relations.png)

1. When the investor invests, their investment goes into the investor stake wallet

2. The Pivot protocol immediately matches that investment, moving the same amount of $UNDEAD into the pool's reserve from the protocol's reserve (not the treasury; the reserve).

Okay, we have $UNDEAD in two places (three if this were an echo-pool). So what? That's where ./otto comes in.

![./otto reserve swaps](imgs/components/02c-otto.png)

Every day, ./otto checks the pool-reserve and converts the $UNDEAD to the pool-assets, at, importantly: the `min_swap`-value (say: $1k).

What does this pool-as-three-wallets give us? Complication? No: simplification.

1. The investors' $UNDEAD is safe. They can withdraw at any time.

2. The reserve is entirely separate from the pool. We're not commingling assets. This is especially important for the echo-pools and for pivot performance calculations.

#### Example

Let's walk through an example, using the BTC+ETH pivot pool.

1. ./otto sees $UNDEAD in the reserves
2. ./otto swaps `min_swap` $UNDEAD to $BTC
3. ./otto swaps `min_swap` $UNDEAD to $ETH
5. ./otto transfers all swapped assets to the pool wallet.

The above swaps will be greatly facilitated by established $UNDEAD LPs. In the event of no $UNDEAD LP, uniswap currently has a fair swap for UNDEAD/ETH at `min_swap` value, so all swaps would start with $UNDEAD -> $ETH, then $ETH -> target asset.

Why DCA at all? Why not just swap all the $UNDEAD to the target assets? A large swap will affect a low liquidity asset's price, such as $UNDEAD, and, if we wait to time the market, we lose out on (much) more profitable pivot-opportunities with the bluechip pivot assets.

## Protocol Liquidity Flow

How does liquidity flow within the Pivot Protocol and why?

### Pivot pools

![Pivot pool liquidity flow](imgs/flows/01-pivot-pools.png)

When a pivot pool completes pivot arbitrage (that is: opens a pivot with a swap
of the principal asset to the pivot asset _then_ closes that pivot with a swap
back), there's a gain of the principal asset, let's say, for example, the 
following pivot occurs:

1. 202a-bb-cc, open pivot: swap 1 $BTC for 18.5 $ETH
2. 202x-yy-zz, close pivot: swap 18.5 $ETH for 1.2 $BTC

The _gain_ from this pivot is 0.2 $BTC. This gain is distributed throughout the
protocol in the following manner (please refer to the diagram, above, for the
distribution-flow).

1. 10% of the gain (in this example, 0.02 $BTC), _in total_, is distributed to
_all_ investors. So, if your investment comprised 10% of the pool, your yield
would be 0.002 $BTC.

2. 10% of the gain (again, 0.02 $BTC) would go into the BTC+ETH echo pool for
pivot arbitrage there to grow the protocol.

3. 40% (e.g.: 0.08 $BTC) _remains_ in the BTC+ETH pivot pool, growing the pool 
and strengthening its pivots.

4. 40% of the gain (again, 0.08 $BTC) goes to the Treasury.

* 0.02 $BTC (investors) + 0.02 $BTC (echo) + 0.08 $BTC (reinvest) + 0.08 $BTC (treasury) = 0.2 $BTC

Q.E.D.

### Echo pools

![Echo pool liquidity flow](imgs/flows/02-echo-pools.png)

Again, please refer to this above diagram for the discussion of echo pool
liquidity flow.

1. 20% of echo pool pivot arbitrage gains goes to the investor (remember,
the echo pool is populated from its pivot pool at 10% of gains, so the echo
pool is much smaller: you're not making more tokens by investing in the echo
pool, generally-speaking).

2. 40% of the echo pool pivot arbitrage gains goes to the treasury.

3. 40% of the echo pool pivot arbitrage gains remain in the echo pool, 
strengthening its pivot arbitrage trades.

### Treasury

![The Treasury liquidity flow](imgs/flows/03-treasury.png)

The Treasury is the repository of the protocol's assets, building liquidity
depth. It serves two functions:

1. Building the wealth of the protocol to be deployed to new pools and new
projects as the protocol sees fit.
2. Disbursing protocol-assets to investors from a safe (read: 'slow' or 'boring')
repository.

Liquidity flows into the Treasury from investors and from the protocol pivot-
and echo-pools. Liquidity flows from the Treasury in the following ways (please
refer to the above diagram):

1. When the Treasury receives gains from any pivot, say, e.g.: $BTC, 10% of
that gain are distributed to all investors.
2. On a regular cadence, say, e.g.: weekly, an annualized 3% of the protocol's
assets are distributed to all investors.

Two notes on 2. above. 

* _Assets_ are distinct from _investments_ in the Treasury. The $UNDEAD tokens 
you, the investor, invest into the Treasury are not disbursed in 2., but, 
instead, are kept in reserve by the protocol.
* '3% annualized' means just that. So, if disbursements are weekly, a 3%
annualized disbursement would be factored for the weekly release, meaning that
1/52nd of that 3% annualized disbursement would be distributed to all investors,
_not_, to be clear here, 3% of the Treasury on a weekly basis, as that would
drain the Treasury's assets quite quickly. The point of the Treasury is to 
build wealth, not to disburse it.

3. As the protocol grows in success, showing the efficacy of the pivot and echo
pools, there will be demand for new pivot pools, both for, say more BTC+ETH 
pivot pools or for pools with other tokens of value, e.g.: $PAXG. An
apportionment of the Treasury will be used to explore new internal income
streams.

4. Pivot arbitrage isn't the last new idea in the Blockaverse. Somebody will
come up with a new approach to investing that uses liquidity in novel ways,
generating new ways to invest. The Treasury will incubate new, promising,
proven ideas in crypto finance.

The latter two (3. and 4.) will come after the Pivot Protocol, itself, has
proven its own resiliency. Also, funding new pivot pools or protocols will not
put a strain on the day-to-day operations of the Pivot Protocol, itself, so:
no investment nor research will be allowed to take more than 10% of the 
Treasury's assets.

## Wat do???

So, how do you invest into the Pivot Protocol? 

1. First, you need $UNDEAD liquidity, so you need to obtain $UNDEAD tokens 
from whichever DEX or CEX provides them. Currently, Uniswap has a fair 
ETH/UNDEAD swap.

2. Choose the pool that suites your investment-aims and tolerance to risk.

3. If you want to profit from pivot arbitrage across all pivot pools, consider
investing into the Treasury.

4. Invest for great joy.

Pivot-trades occurs at most once per day per pool, so you don't need to 
machinegun refresh your browser. Check the protocol once per day, invest
where you will, harvest your _real_ yields, then spend the rest of your day,
living your life, ...

... as you do.

![Ride that pivot-curve!](imgs/01-btc-eth-ratio.png)

_fin._

[Cwædon þæt he wære](https://www.hieronymus.us.com/latinweb/Mediaevum/Beowulf.htm#X43) wyruldcyning, ...

![Cwædon þæt he wære wyruldcyning](imgs/zz-Cwædon.png)
