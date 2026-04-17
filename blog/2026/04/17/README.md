# Synthetics

G'day, pivoteurs!

![`dusk` report](imgs/01a-dusk.png)

`dusk` calls for $71k in close pivots.

Meanwhile, on @Cardano, @Indigo_protocol has some activity in synthetics.

![Synthetics on Indigo](imgs/01b-indigo.png)

I'm going to explore synthetics today. I have $5k in close pivots in the 
synthetics markets, so: here we go!

## Indigo

For the synthetic-staking on @Indigo_protocol, I harvest:

![Harvest iUSD ADA](imgs/02a-iUSD.png)

* 276 $ADA for 59 $iUSD ($11 gain)

![Harvest iBTC ADA](imgs/02b-iBTC.png)

* 903 $ADA for 0.00277 $iBTC ($24 gain)

![Harvest iETH ADA](imgs/02c-iETH.png)

* 104 $ADA for 0.01178 $iETH ($1 loss)

Overall, a net $34 gain for $7,500 staked.

So ... 'meh?' is my evaluation so far.

## Synthetic Pivots

![iBTC-swap on MinSwap](imgs/04a-m-btc.png)
![iETH-swap on MinSwap](imgs/04b-m-eth.png)

Now, for the ADA-pivots, both the 

* ADA-on-BTC and
* ADA-on-ETH

pivots return less than 10% gain (or even A LOSS!?!) because the slippage 
on @MinswapDEX, and it's WORSE on @Indigo_protocol!

![iBTC-swap on Indigo](imgs/04c-i-btc.png)
![iETH-swap on Indigo](imgs/04d-i-eth.png)

If you can't swap $2.5k of $BTC, you have to ask if synthetics are viable on 
Cardano.

### Analysis

That doesn't mean that synthetics are bad. Other protocols have done them, and 
done them well, but it does mean that maybe Cardano isn't a blockchain to 
trade, due to slippage.

![Indigo TVL](imgs/05-indigo-tvl.png)

Why is lack of liquidity a problem on Cardano? There's $8.7M liquidity 
on @Indigo_protocol! Baffling!

### No Pivots on Cardano due to slippage

At any rate, here's my report-card on the ADA-pivots:

![No fulfilled pivots on Cardano](imgs/06-f-ada.png)

* $5k is taken off the table because of slippage

@Cardano @Indigo_protocol @MinswapDEX: please address this slippage issue for 
synthetic trades.

### Post-transaction amount changes on MinSwap

This is how bad, and how stupid, trading is on Cardano:

I submitted a trade-request to @MinswapDEX 

![Requested trade accepted on MinSwap](imgs/07a-submit.png)

* 903 $ADA -> 0.032 $iBTC

Instead, MinSwap executed

![Trade changed after transaction accepted](imgs/07b-traded.png)

* 841.6 $ADA -> 0.029 $iBTC

MinSwap, really? If you accept my trade-request (transaction confirmed), you 
can't change it after.

### MinSwap refused trade

![MinSwap refused $iUSD trade](imgs/08a-no-trade-minswap.png)

Then @minswap flat-refused to trade $ADA for $iUSD, ... even though they 
provided the interface to set up the trade. Very puzzling!

![Trade submitted on Indigo](imgs/08b-submit.png)
![Trade executed on Indigo](imgs/08c-traded.png)

At least for @Indigo_protocol, they traded the amount $ADA I submitted for the 
amount of $iUSD I requested.

You see how that works, MinSwap?

