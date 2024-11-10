# Funding new pivot pools

> synopsis: You've [set up a new pivot-pool](pool-setup.md) with its three wallets. Now: how do you determine who funds how much into the pool, and what does that say about the pool's market capitalization. An HOWTO article.

You've [set up a new pivot pool](pool-setup.md), say, for example, the ETH-BTC pivot pool. Great!

Now what?

Now we fund it.

How?

Good question!

## HOWTO Fund new pivot pools

The agreement between Wagyu games and the Pivot Protocol is that:

* Pivot protocol funds 30% of the pivot pool
* Wagyu games funds 20% of the pivot pool

Okay, that is easy. I fund 30%; Wagyu games funds 20%: we get the market capitalization when we take those two together and double that. That is: everybody else gets to stake another 50%, and that's the pool's market cap.

Let's work through the ETH-BTC pivot pool. Let's say we put a market capitalization of $10,000.00, which, at today's price of $UNDEAD ($0.01336), is a market capitalization of 748,500 $UNDEAD.

This means 

* I fund the ETH-BTC pivot pool 224,550 $UNDEAD
* Wagyu games funds the pool 149,700 $UNDEAD

And Bob's your uncle.

The. End.

... but not quite, my friends!

## The Echo pool

Because, recall the [structure of the protocol](https://github.com/pivoteur/biz/tree/main?tab=readme-ov-file#pivot-protocol-ecosystem)! The pivot pool has the associated [echo pool](https://github.com/pivoteur/biz/tree/main?tab=readme-ov-file#2-the-echo-pools).

By policy, I invest 10% of what I invested into the pivot-pool into the echo pool, and Waygu games, by agreement, invest 20% of the echo pool, as well, so:

* I fund 22,455 $UNDEAD into the echo pool
* Wagyu games funds 14,970 $UNDEAD into the echo pool

And, per the protocol, there's one more investment round.

## Treasury

The [Treasury](https://github.com/pivoteur/biz/tree/main?tab=readme-ov-file#3-the-treasury-norge) also receives gains from all pivot pools and the echo pool, so stakers gain from those gains.

By policy, I invest 5% into the treasury, so I'll be adding 5% more $UNDEAD for each newly created and funded pivot pool. Wagyu games follows suite with their 20% investment.

* I fund the treasury with 11,227 $UNDEAD
* Wagyu games funds the treasury with 7,485 $UNDEAD.

## Summary

So, for each newly created pool initial funding flows into that pool with the Pivot protocol contributing 30% of the market capitalization and Wagyu games contributing 20% of that market capitalization, then funding flows into the echo pool at 10%, and finally it flows into the treasury at 5%.
