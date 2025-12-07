# Completing `baewulf` by doing the work

2025-12-06

We have one more thing to do to make the close-side of baewulf complete: 
aggregate tokens-to-swap, but to do that, we need to distinguish on which 
blockchains the coins are.

TODO that we need to add blockchain info to pivots opened, so we may as well 
GET TO WORK!

# Step 1: bae

![`bae`-watch, ... I mean: `bae`-run, ... that's what I meant!](imgs/01-bae.png)

Today's quotes for tokens pivoted: collected! ✅

# Step 2: wulf, jr (`hound`, actually)

![`hound` recommendations](imgs/02-hound.png)

I run `hound` against the open pivots and it comes up with three recommendations:

* BTC+UNDEAD (on Avalanche)
* HBAR+USDC (on Hedera)
* UNDEAD+USDC (on Avalanche)

So! Work to be done! I'll go through EVERY pivot pool and add blockchain info

## Human-readable `hound`-runoff 

BTW, the `hound`-runoff is CSV so is human-readable from a spreadsheet.

![`hound`-report](imgs/03-tabled.png)

Here's what the output looks like, cleaned-up.
# Vote for $UNDEAD LPs on Blackhole 

2025-12-06 

A new day; a new Epoch on @BlackholeDex. 

Reminder to go [vote](https://blackhole.xyz/vote) for the @UndeadBlocks $UNDEAD liquidity pools on that DEX. 

![Blackhole DEX voting page](imgs/05a-vote.png) 
![Vote for $UNDEAD LPs](imgs/05b-voted.png) 

[HOWTO vote instructions](https://x.com/pivocateur/status/1945637734682341791) 

#IVotedForUNDEAD 

# PIVOTS 

## BTC+ETH 





No close pivots. 











## Open BTC+ETH pivots 

![BTC+ETH Ratio](imgs/06a-ratio.png) 
![Middling δ](imgs/06b-delta.png) 

The meh δ makes no call, but I open an BTC-on-ETH pivot, anyway. 

![Open BTC pivot](imgs/06c-open-btc-pivot.png) 

I also open an ETH-on-BTC pivot. 

![Open ETH pivot](imgs/06d-open-eth-pivot.png) 











### Move pivots to Hedera 

* I swap 0.0554 BTC to USDC 



* I swap 1.1376 ETH to USDC. 


![Send to Coinbase](imgs/07a-sned.png) 
![Swap to HBAR](imgs/07b-swap-to-hbar.png) 

and bridge that liquidity to Hedera as HBAR, where I swap back to BTC and ETH 

![Swap to BTC](imgs/07c-swap-to-btc.png) 
![Swap to ETH](imgs/07d-swap-to-eth.png) 

The BTC+ETH pivot pool composition and γ-apportionment are as charted. 

![The BTC+ETH pivot pool composition](imgs/08a-comp.png) 
![The BTC+ETH pivot pool γ-apportionment](imgs/08b-apport.png) 

You see that the assets' blockchains are now part of the pool's composition-data.


