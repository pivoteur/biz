# Pivot Pools vs Liquidity Pools

HWÆT, pivoteurs!

* Liquidity pools have "impermanent loss" (IL)

* Pivot pools are the exact opposite: they have "permanent gains" (PG)

![Liqudity pool with Impermenant Loss](imgs/01a-lp.png)

* BTC/USDt on @KyberNetwork is making 9% on @binance with the risk of IL.

![Pivot pools](imgs/01b-pivot.png)

* BTC+USDC pivot pool is making 15% on https://pivoteur.github.io/pools.html 
with PG. 

# Pivots

## BTC+USDC

![BTC/USDC ratios](imgs/02a-ratio.png)
![BTC/USDC delta](imgs/02b-delta.png)
![Open BTC-on-USDC pivot](imgs/02c-open-btc-on-usdc-pivot.png)
![Open USDC-on-BTC hedge](imgs/02d-open-usdc-on-btc-hedge.png)

The protocol opens a BTC-on-USDC pivot and, at the same time, a USDC-on-BTC 
hedge upon reviewing the BTC/USDC ratio and δs. 

## ETH+UNDEAD

![ETH/UNDEAD ratios](imgs/03a-ratio.png)
![ETH/UNDEAD delta](imgs/03b-delta.png)
![Open ETH-on-UNDEAD pivot](imgs/03c-open-eth-on-undead-pivot.png)
![Open UNDEAD-on-ETH pivot](imgs/03d-open-undead-on-eth-pivot.png)

I also open an ETH-on-UNDEAD pivot and an UNDEAD-on-ETH pivot as the 
indicators make no call either way. 

## BTC+UNDEAD

![BTC/UNDEAD ratio](imgs/04a-ratio.png)
![BTC/UNDEAD delta](imgs/04b-delta.png)
![Open UNDEAD-on-BTC pivot](imgs/04c-open-undead-on-btc-pivot.png)

I open an UNDEAD-on-BTC pivot. 

## UNDEAD+USDC

![UNDEAD/USDC ratios](imgs/05a-ratio.png)
![UNDEAD/USDC delta](imgs/05b-delta.png)
![Open UNDEAD-on-USDC pivot](imgs/05c-open-undead-on-usdc-pivot.png)
![Open USDC-on-UNDEAD pivot](imgs/05d-open-usdc-on-undead-pivot.png)

I open both an UNDEAD-on-USDC and a USDC-on-UNDEAD pivots. 

