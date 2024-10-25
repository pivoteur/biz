2024-10-25: ./dawn has pivot-recommendations for both the BTC+ETH pivot pool and the BTC+PAXG+BNB pivot pool.

# BTC+ETH pivot pool

For the BTC+ETH pivot pool, ./dawn recommends a 0.0227 BTC -> ETH swap. The charts support this. 

![./dawn BTC recommendation](imgs/01a-dawn-btc-rec.png)
![BTC/ETH chart](imgs/01b-btc-eth.png)

./dusk rejects the close-pivot as it's "only" 111% APR gain (7% ROI) (pink), so it opens a new BTC-on-ETH pivot (cyan). Note that uniswap's swap is favorable to us, giving us MORE ETH than calculated (green cell). 

![No close pivot](imgs/02a-no-close-pivot.png)
![Open BTC-on-ETH pivot](imgs/02b-open-btc-pivot.png)

BTC+ETH pivot pool after open-pivot trade.

![BTC+ETH pivot pool](imgs/03a-btc-eth-pivot-pool.png)
![Table of pool after open BTC-on-ETH pivot](imgs/03b-btc-eth-pivot-table.png)

# BTC+PAXG+BNB pivot pool

./dawn has 2 recommendations for the PAXG pivot pool. Let's take each in turn.

![./dawn PAXG recommendations](imgs/04-dawn-paxg-recs.png)

## BTC -> PAXG

First, BTC -> PAXG. The δ is smallish, so ./dusk vetos a close pivot (negative ROI) and also vetos an open pivot (swap < min_swap)

![BTC/PAXG chart](imgs/05a-btc-paxg.png)
![No close pivot](imgs/05b-no-close-pivot.png)
![No open pivot](imgs/05c-no-open-pivot.png)

## BTC -> BNB
Second, BTC -> BNB. ./dusk does not close any open pivots, so we open a BTC-on-BNB pivot ... the swap is against us this time, both on uniswap and on pancakeswap.

![BTC/BNB chart](imgs/06a-btc-bnb.png)
![No close pivot](imgs/06b-no-close-pivot.png)
![Open BTC-on-BNB pivot](imgs/06c-open-btc-pivot.png)

# The Pivot Advantage

The BTC+PAXG+BNB pivot pool with the pivot-advantage. Opening pivots puts pivots in the pipeline, closing pivots captures the pivot-gains.

![PAXG pivot pool](imgs/07a-paxg-pivot-pool.png)
![The Pivot trade advantage](imgs/07b-pivot-advantage.png)

