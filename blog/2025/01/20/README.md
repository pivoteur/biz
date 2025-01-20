# Development

2025-01-20

Good morning, all!

## Work completed

Pool-indexing is now data-driven, meaning:

![Data-driven indexing](imgs/01a-pool-indexing.png)

* we get what we got before, now with accurate and up-to-date measures

![Adding new pools](imgs/01b-automated.png)

* right) we can now add pools ... 'automagically' by updating links and references in the data now.

## TODO

There's work to be done on and from this page:

1. The 'automagically' adding new pools requires manual intervention for the landing-page of each of these pools. These pages should be templated.

2. The non-pool stakes (treasury and echo pool) need to be automated.

With a 2-line addition to the pools.html javascript, I now how non-pool stakes (treasury and echo) automated and data-driven. 

![Treasury and echo pool indexing now automated](imgs/02-non-stake.png)

So 2. goes from TODO to TODOne! 

# Pivots

Now we have the pivot pool indices data-driven, let's see what pivots to execute today

## BTC+BNB

There's a call to close an open BNB-on-BTC pivot, which I do

![Close BNB-on-BTC pivot](imgs/03a-close-bnb-on-btc.png)

* actual ROI: 12.93% / 104.87% APR projected 

The δ here calls for opening a BTC-on-BNB pivot, but all $BTC is committed.

![Positive BTC+BNB δ](imgs/03b-pos-δ.png)

The BTC+BNB pivot pool composition and γ-apportionment stands as charted. 

![BTC+BNB composition](imgs/04a-comp.png)
![BTC+BNB γ-apportionment)(imgs/04b-apport.png)

Uploading the BTC+BNB pivot trading history to [the Pivot Protocol](https://pivoteur.github.io/#) automatically updates tracking on the site. #datadriven 

## BTC+ETH

No good closes for open BTC+ETH pivots. 

![BTC+ETH positive δ](imgs/05-pos-btc-eth-δ.png)

The δs recommend opening a BTC-on-ETH pivot, however, all BTC is currently committed to open pivots already. 

## BTC+DOGE

No good closes for BTC+DOGE pivots. 

![BTC+DOGE positive δ](imgs/06-pos-btc-doge-δ.png)

We do have a positive δ, however, it's mid and I have an open pivot in this δ-band, so I leave this pool as-is. 

## BNB+LTC

I close a BNB-on-LTC pivot to good results:

![close BNB-on-LTC](imgs/07a-close-bnb-on-ltc.png)

* actual ROI: 21.20% / 1105.42% APR projected

The negative δ calls to open a LTC-on-BNB pivot, so I do just that. 

![Negative BNB+LTC δ](imgs/07b-neg-δ.png)
![Open LTC-on-BNB pivot](imgs/07c-open-ltc-on-bnb.png)

The BNB+LTC pivot pool's composition and γ-apportionment is as charted.

![BNB+LTC composition](imgs/08a-comp.png)
![BNB+LTC γ-apportionment](imgs/08b-apport.png)

Once I upload BNB+LTC pivot pool's historical trade data, the pool's state will be reflected on the [protocol](https://pivoteur.github.io/#).

## BNB+LINK

No good close pivots today. 

![Negative BNB+LINK δ](imgs/09a-neg-δ.png)
![Open LINK-on-BNB pivot](imgs/09b-open-link-on-bnb.png)

The negative δ calls to open a LINK-on-BNB pivot, and, after transferring some $BNB from the treasury to cover gas, I open a new pivot. 

The BNB+LINK composition and γ-apportionment are as charted.

![BNB+LINK composition](imgs/10a-comp.png)
![BNB+LINK γ-apportionment](imgs/10b-apport.png)

## LTC+LINK

There are no good close pivots today and the δ-band is already covered by an open pivot (the first open pivot, in fact).

![LTC+LINK δ](imgs/11a-meh-δ.png)

The LTC+LINK composition and γ-apportionment are as charted. 

![LTC+LINK composition](imgs/11b-comp.png)
![LTC+LINK γ-apportionment](imgs/11c-apport.png)

## AVAX+QI

There's a killer close on a QI-on-AVAX pivot:

![close QI-on-AVAX pivot](imgs/12a-close-qi-on-avax.png)

* actual ROI: 20.29% / 176.37% APR projected
* or: 7k $QI -> $AVAX -> 8.4k $QI.

WOOT!

![Positive AVAX+QI δ](imgs/12b-pos-δ.png)

The positive δ favors opening an AVAX-on-QI, but all $AVAX is currently committed to open pivots.

Composition and γ-apportionment as charted:

![AVAX+QI composition](imgs/12c-comp.png)
![AVAX+QI γ-apportionment](imgs/12d-apport.png)

# finis

All data uploaded to the [protocol dapp](https://pivoteur.github.io/#). This concludes today's activities.
