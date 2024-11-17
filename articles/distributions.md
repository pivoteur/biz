# Computing Pivot Distributions

> synopsis: Distributing pivot gains can be a rather complicated affair, as distributions from the pool-type, the treasury, and amplified returns to stakers must all be taken into consideration. Non-pre-computed distributions can entail 9 or more transactions. On Ethereum, with transaction fees going into the dollar-range – and multiples of that! – each transaction eats into the pivot gains, so, pre-computing distribution amounts and minimizing the number of distributions *a priori* becomes paramount.

## The Problem

Ethereum transaction fees.

## The solution

Pre-computation of distributions, eliminating 'call-back'-distributions

## The Problem, II

Pre-computing isn't easy.

## The Solution, II

This article.

## Context

Before we look at precomputing distributions, let's look at what distributions of pivot gains on the Pivot Protocol look like now, that is: not-pre-computed.

For context, distribution-flow is discussed in the 
[Pivot Protocol whitepaper](../README.md#protocol-liquidity-flow).

Let's take an example from today, 2024-11-17.

Close echo pivot generated the following gains:

![Echo pivot gains](imgs/dist/01-echo-pivot-gains.png)

* 2,733 $UNDEAD
* 0.00947 $ETH

### Consideration: transacting $UNDEAD costs *a lot* more

First, know that every non-$ETH transaction costs more gas, so, it is advantageous to convert to $ETH before we transfer any liquidity, ... BUT!

We have a pivot gain of (primarily:) $UNDEAD, so we want to keep the gain that *stays* in the Echo Pool as $UNDEAD.

## Distribution Flow

Let's take a distribution flow from the gains froman Echo pool pivot close.

> note: Echo pool gains distributions are different than pivot pool distributions.

1. <del>We have the gains from the above, we transfer 100% of those gains to the `distributor`-dapp.</del>

> please note (1): this is already complicated, because transferring $UNDEAD costs *much* more than transferring $ETH, so it makes sense to convert all $UNDEAD to $ETH before transferring liquidity.

> please note (2): *BUT* we want to keep the $UNDEAD gains that remain in the echo pool as $UNDEAD, because, after all, that's 
[the entire point of the echo pool](../README.md#2-the-echo-pools)


