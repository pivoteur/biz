# PIVOTS 

## BTC+ETH 

* There are 32 open pivots for the BTC+ETH pivot pool. 
* The last entry is on 2025-11-23. 
* Recommendations are made for token quotes on 2025-11-26. 

> No close pivot recommendations for BTC+ETH pivot pool. 

### Transfer pivots to Hedera

Now that I've opened these pivots, let's move them to @hedera.

Easier said than done.

First thing's first. 

* I convert the $BTC and $ETH to $USDC, 

![Swap BTC to USDC](imgs/02a-swap.png)
![Swap ETH to USDC](imgs/02b-swap.png)

* then send that liquidity to @coinbase. 

![Receive addy on Coinbase](imgs/02c-receive.png)
![Send liquidity to Coinbase](imgs/02d-sned.png)

### Swap to $HBAR

Next, I swap the $USDC to $HBAR to send to @hedera, right?

Here's the thing, the @coinbase swap yields 68,260 $HBAR, 

![Coinbase swap to $HBAR](imgs/03a-coinbase.png)

...but the @SaucerSwapLabs of the same amount of $USDC yields 68,610.

![Saucerswap to $HBAR](imgs/03b-saucer.png)

That's too much of a hit.

Or is it?

If I bridge via @HashportNetwork, I lose $50, anyway.

![Hashport bridge](imgs/03c-hashport.png)
![Saucerswap with bridged $USDC](imgs/03d-saucer.png)

### BTC+ETH pivots on Hedera

The result is that a @coinbase swap with no bridging is within $10 of bridged assets to @hedera, so I swap to $HBAR on Coinbase and then send that liquidity to Hedera.

![Swap to $HBAR on Coinbase](imgs/04a-coinbase.png)
![Send $HBAR to Hedera](imgs/04b-sned.png)

Once there (nearly instantanious), I swap to $BTC and $ETH.

![Swap to BTC](imgs/04c-btc.png)
![Swap to ETH](imgs/04d-eth.png)

The BTC-on-ETH and ETH-on-BTC pivots that are now on @hedera are marked with a gray highlight in the open-pivot log.

![Gray highlights for pivots on Hedera](imgs/05-gray.png)

BTC+ETH pivots are now on @hedera.

The BTC+ETH pivot pool composition and γ-apportionment are as charted. 

![The BTC+ETH pivot pool composition](imgs/06a-comp.png) 
![The BTC+ETH pivot pool γ-apportionment](imgs/06b-apport.png) 

