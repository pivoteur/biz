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
[Pivot Protocol whitepaper](../README.md#protocol-liquidity-flow)

Let's take an example from today, 2024-11-17.

Close echo pivot generated the following gains:

![Echo pivot gains](imgs/dist/01-echo-pivot-gains.png)

* 2,733 $UNDEAD
* 0.00947 $ETH

### Consideration: transacting $UNDEAD costs *a lot* more

First, know that every non-$ETH transaction costs more gas, so, it is advantageous to convert to $ETH before we transfer any liquidity, ... BUT!

We have a pivot gain of (primarily:) $UNDEAD, so we want to keep the gain that *stays* in the Echo Pool as $UNDEAD.
