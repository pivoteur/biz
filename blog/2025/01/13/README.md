# Audit, part II, 2025-01-13

## $UNDEAD

Yesterday we left off auditing the tabs of the Pivot protocol dapp, but there is data on the dapp not being displayed, and that is the $UNDEAD 24h-volume, @coingecko place, and price.

![UNDEAD coingecko place](imgs/01a-undead.png)
![UNDEAD price](imgs/01b-undead.png)
![UNDEAD market cap](imgs/01c-undead.png)
![UNDEAD 24h-volume](imgs/01d-undead.png)

I do track these internally. Should the dapp have a page for this?

# Balanced (fiat) account

A point of order.

The Pivot Technologies operating (fiat) account is balanced, because, yes, a protocol needs (fiat) money to operate.

![Balanced Checkbook](imgs/02-account-balanced.png)

# Audit, reprise

## Summary page automation

Back to part II of the audit, which is to focus on each pivot pool.

![Summary pool page, missing pivot pools](imgs/03a-missing-pools.png)

You see from the pools summary page, some pivot pools are missing, as the summary page is (currently) entirely manual.

I've added a 'security'-column to assist parsing pivot pools from address-data. 

![Security column to automate pivot pool UX](imgs/03b-security-col.png)

## BTC+ETH

First pool, BTC+ETH

![BTC+ETH broken UX](imgs/04a-no-btc-eth-ux.png)

The UX for this pivot pool is broken. TODO: FIXME!

An ETH-on-BTC pivot has a favorable close, gaining:

* actual ROI: 7.98% / 59.41% APR projected

or 0.05 $ETH -> $BTC -> 0.054 $ETH

![close ETH-on-BTC pivot](imgs/04b-close-eth-on-btc.png)

The δ is strongly positive, too, so I open a BTC-on-ETH pivot here. 

![Positive δ](imgs/04c-pos-δ.png)
![Open BTC-on-ETH pivot](imgs/04d-open-btc-on-eth.png)

The BTC+ETH pivot pool composition and γ-apportionment.

![BTC+ETH composition](imgs/05a-comp.png)
![BTC+ETH γ-apportionment](imgs/05b-apport.png)

I've uploaded the BTC+ETH data to the dapp, so when I templatize the pivot pools, the UX will update automatically upon upload.

## BTC+BNB

Next, BTC+BNB.

The UX is half-working: Radar chart works, bar chart does not.

![BTC+BNB Radar chart](imgs/06a-btc-bnb-radar.png)
![no BTC+BNB bar chart](imgs/06b-btc-bnb-no-bar.png)

There are no advantageous close pivots today, and the δ is meh, so I leave the pool as-is. 

![BTC+BNB meh δ](imgs/06c-meh-δ.png)

## BTC+DOGE

Next, BTC+DOGE

![No BTC+DOGE UX](imgs/07a-no-btc-doge-ux.png)

The BTC+DOGE pivot pool UX is broken. TODO: FIXME!

There are no advantageous close pivots, and the δ is meh, so I open no new pivots.

![Meh BTC+DOGE δ](imgs/07b-meh-δ.png)

Sometimes doing nothing makes the most sense in a market when doing pivot arbitrage.

## BNB+LTC

The next three pivot pools have no UX ... yet.

BNB+LTC

There's no good close pivot, but the δ is now positive, so I open a BNB-on-LTC pivot.

![Positive δ](imgs/08a-pos-δ.png)
![open BNB-on-LTC pivot](imgs/08b-open-bnb-on-ltc.png)

The pool composition and γ-apportionment are as charted (manual now; soon to be data-driven and automated). 

![BNB+LTC composition](imgs/08c-comp.png)
![BNB+LTC γ-apportionment](imgs/08d-apport.png)

## BNB+LINK

![BNB+LINK chart](imgs/09-bnb-link.png)

There are no good close pivots here. The δ is positive, but I don't have any BNB to swap to LINK to start a BNB-on-LINK pivot, so I do nothing here.

## LTC+LINK

![LTC+LINK chart](imgs/10-ltc-link.png)

No good close pivots here, and, even though we have a positive δ, we already have an open LTC-on-LINK pivot open around this band, so we're good here.

## AVAX+QI

![AVAX+QI Radar chart](imgs/11a-avax-qi-radar.png)
![AVAX+QI Bar chart](imgs/11b-avax-qi-bar.png)

Finally, a working pivot pool UX, with both radar and bar charts working. This, then, becomes our template for other pivot pools (although radar panel could be smaller).

There are no good close pivots, and the positive δ indicates sell $AVAX, but all $AVAX is committed.

![Positive δ](imgs/11c-pos-δ.png)

This concludes the audit.

Tomorrow I'll begin fixing the issues identified here.
