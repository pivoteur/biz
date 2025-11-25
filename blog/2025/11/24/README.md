# BRIDGING
## Bridging Liquidity from Avalanche to Hedera

2025-11-24

Okay, we're going to work toward transitioning funds from @avax, where we're currently pivoting, to @hedera, where we go live with the Pivot protocol, end-of-year 2025.

I know of three ways to move liquidity from @avax to @hedera:

### SimpleSwap

1. @avax $USDC -> @hedera $HBAR using @SimpleSwap_io, which has its own bridge, with its own associated (invisible) fees that show up as less $HBAR received.

![Bridge liquidity using SimpleSwap](imgs/01-simple.png)

1,000 @avax $USDC results in 6,601 @hedera $HBAR

### Hashport bridge

2. @avax $AUSD -> @ethereum $USDC using @KyberNetwork

![Bridge to Ethereum using Kyber DEX](imgs/02a-kyber.png)

  -> @hedera $USDC using @HashportNetwork (5 $USDC fee)

![Bridge to Hedera using Hashport](imgs/02b-hashport.png)

Then, swap to $HBAR using either:

* @SaucerSwapLabs, which has the most liquidity, yielding 6,643 $HBAR; or,

![SaucerSwap](imgs/02c-saucer.png)

* @HSuiteNetwork, yielding 6,541 $HBAR 

![HSuite](imgs/02d-hsuite.png)

(102 $HBAR less! or a $19 hit!)

### Coinbase

3. via @coinbase: @avax $USDC -> @coinbase swap to $HBAR

![Send $USDC to Coinbase from Avalanche](imgs/03a-send-from-avax.png)
![Swap to HBAR](imgs/03b-coinbase.png)

1,000 $USDC -> 6,827 $HBAR

### Recap

But it's been hours since the last set of swaps, so the revised swaps are now:

* Saucer: -> 6,823.12

![Saucer swap](imgs/03c-saucer-update.png)

* Simple: -> 6,806.38

![Simple swap-and-bridge](imgs/03d-simple-update.png)

* and coinbase, as you see: -> 6,827

Coinbase is the winner.

