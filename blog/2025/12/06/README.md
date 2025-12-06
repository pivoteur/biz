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
