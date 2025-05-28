# Working Agreement, draft, 2025-05-28

## Legalize Terms

* I/me: Pivot Technologies, LLC
* You/you: Wagyu Games
* We/us: You and I
* party: You or I

# Essentials

## Roles

* I will provide daily reports and pivots and half the working liquidity as
UNDEAD tokens, a pivot pool address and a wash account address on the alt chain.
* You will provide half the working liquidity as pivot/protocol tokens and the 
code of an automaton to trade, then to trade-back, my manual daily pivot 
activity on a configurable periodic basis, snapshotted daily at a configurable
time.
* We will snapshot UNDEAD's rank, quote, market cap, and 24-hour volume at the
start of the effort
* We meet regularly to measure the effort's success and adjust as necessary
* Either party may terminate this agreement. I consider it a courtesy for both
parties to discuss the reason for termination and the time of termination, or
we may continue this for as long as we shall live if so amendable.

## Terms of Agreement

* UNDEAD pivot trading on an alt blockchain we agree to
* Establish a (new) pivot pool address under my control (the 'pivot pool')
* Establish a (new) wash address (the 'wash account'); described below
* You are to provide agreed-upon amount of pivot tokens to the pivot pool and
10% of pivot tokens to the wash address
* I am to provide an equal dollar-amount of UNDEAD tokens to the pivot pool and
10% of that dollar-amount to the wash address
* You will receive 40% of the pivot-gains at the close of each pivot
* I will also receive 40% of the pivot-gains
* The pivot pool will retain 20% of the pivot-gains
* Wagyu to provide an address for me to send the pivot-gains
* Wagyu to provide code to automate the execution of the hourly trade/trade-back
on the wash account (discussed below)

## Area to hash out

Who controls the wash account? I recommend I control the wash account, so that 
I could run the automaton periodically (hourly, to start with), and monitor and
adjust as necessary.

## Measurement

We accomplish this aim how? I propose the following measures

* UNDEAD 24-hour volume
* UNDEAD price and market cap
* UNDEAD ranking on coingecko

We take a snapshot at the beginning of this working agreement of those measures
and we meet regularly and compare current measures to those of the inception
of this work-effort.

# Discussion

## Purpose

UNDEAD can be revitalized. I completed a study of UNDEAD volume vs price showing
there is some correspondence between the two. As of today, UNDEAD's trading
volume is ~$220k/day, so here's what I propose:

## Proposal

UNDEAD's price can increase on increased 24-hour trading volume. A way to 
increase trading volume is by creating and activating UNDEAD pivot pools on
alt-chains (where transaction fees are less than $1-per).

If, for example, a $10k AURORA+UNDEAD pivot pool ($5k of AURORA and $5k of 
UNDEAD) address is established on Aurora virtual chain, a pivot for the day 
would be $1k (say AURORA-on-UNDEAD) and the corresponding hedge would be $500
(in this case: UNDEAD-on-AURORA).

This pivot-and-hedge represents $1.5k, which is less than 1% 24-hour volume,
however, I also propose a wash address be established of 10% of each token.
This account would take the trades from the pivot pool address after (say)
midnight GMT, and, every hour duplicate those trades, then immediately trade
back, with a net-zero change in wallet composition, BUT it would add $1.5k
in trades per hour. These (net-zero) trades combined with the pivot-and-hedge
on the pivot pool address would contribute a total of $36k to the 24-hour
trading volume, which is a 15% increase in the daily trading volume. We do this
every day, we move UNDEAD up the ranks (from its current position on coingecko
at 7622), we increase its volume, we get more eyes watching UNDEAD as a 
token-of-value, which, correspondingly, increases price-valuation of the 
UNDEAD token.

## Aim

To be clear, the aim of this working agreement is to rebuild stability of the
UNDEAD token and also to capture more value for the token-holders, which include
us, which form the majority holders of the token. This incidentally benefits
any and every holder of the UNDEAD token, current and future.

## Prerequisits

For this agreement to succeed, we need an environment amendable. I foresee such
an environment being:

* an alt-blockchain with transaction fees less than $1-per.
* LP(s) on the DEX where we execute the trades that is funded such that slippage
on trades is less than 5% per trade, either way.
* A bridge from Ethereum to the alt-blockchain that allows me to transfer the
UNDEAD in my custody to the alt-blockchain without me needing to trade to an
intermediary token (such as ETH or the protocol token or USDC) in order to
materialize the UNDEAD on the alt-blockchain (tl;dr: I need to get the UNDEAD
on the alt-blockchain without catastrophic damage to the transferred amount)
* I need to use all the UNDEAD at my disposal for this effort, this entails me 
*terminating* all pivot pools. Why? The previous effort was to prove pivoting
works (it does) and to prove UNDEAD pivoting works and is profitable (it is).
Advancing the pivot protocol while UNDEAD is unstable is not prudent; therefore,
I recommend shutting down the pivot protocol for now, focusing all our efforts
in revitalizing the UNDEAD token, *then* reinstating parts of the pivot protocol
into the UNDEAD site in a gradual, measured approach, using a stabilized UNDEAD
token as its protocol token.
* I donated all tokens pivoted, so those tokens that are not UNDEAD will be 
returned to me. *ALL* UNDEAD collected from pivot pools, including all gains, 
will be used for the purposes of this agreement.
* I need to get familiar with the alt-chain selected. The most immediately
promising prospects are Aurora virtual chain (from NEAR) and Avalache. I'm 
already familiar with Avalanche, but I have no experience with Aurora, so I'm
going to set up several pivot pools on Aurora to become familiar with that
environment.
* I am not capable of executing wash-trades/trades-back every hour every day.
I need you to create an automaton that:

1. at time x every day (say midnight GMT), observes all trades that occurred
on the pivot pool address
2. at every time, t,  after that (say: t is 1 hour), executes those trades, 
then executes the trades-back on the wash wallet address

n.b.: 

1. only the trades, not transfers into and out of the pivot pool address
2. x and t need to be configurable, either by a property file or via variables
that I have access to.
3. The wash wallet, since trades are both open and close pivots, will profit
from the pivots, just as the pivot pool does, so the wash wallet will gain
value over time, but, since it's 10% the size of its corresponding pivot pool,
I think keeping everything on the wash wallet makes sense, housekeeping-wise.

* the reason why I need you to create this automaton is that I execute trades
manually and have no experience executing trades via code. I think you can
come up with this automaton much more quickly than I can.

## Case-studies / Further study

* [UNDEAD volume-v-price correspondence](/articles/undead-price-v-volume-study.md)
  * To be studied: 24-hour volumes of tokens at rank 5000, 2500, 1000.
  * To be studied: UNDEAD price-equivalents at those rankings

* I will take on the efforts of those above studies and publish and share my
results.

## Caveats

* Pivot arbitrage is 'slow' as measured in 'cryptocurrency-time.'
* My aim is to:
  * firstly, increase UNDEAD's 24-hour trading volume by 10%
  * secondly, get UNDEAD to be ranked above the top-5000 traded crypto, as
measured on coingecko

Both of these are going to take time; they are not going to happen overnight.

* Further goals
  * Get UNDEAD to a $0.005 price-point (a 'ha'-penny')
  * Get UNDEAD to 1¢-per
  * Get UNDEAD to ...? I'd like to get us back to 15¢ and higher, eventually,
but we have to achieve the first two further goals before that moon-shot.

# Conclusion

* We do pivots and wash trades on an alt blockchain
* you provide the pivot/protocol token; I provide the UNDEAD token in equal
measure
* We snapshot UNDEAD's market cap, price, 24-hour volume and rank at the start
* We meet regularly to measure success and adjust as necessary.
* We lather, rinse, repeat for fun and profit for much great joy.

