# 2025-06-28 Status of $UNDEAD 

![$UNDEAD rank](imgs/01a-rank.png) 
![$UNDEAD quote](imgs/01b-quote.png) 
![$UNDEAD market captalization](imgs/01c-cap.png) 
![$UNDEAD 24-hour volume](imgs/01d-vol.png) 

* rank: 8065 
* quote: $0.00226 
* market cap: $33,916 
* 24-hr volume: $110,772 (δ: $3,069 ) 

When we get LPs funded on multiple blockchains, what will $UNDEAD look like? 

[$UNDEAD data source](https://www.coingecko.com/en/coins/undead-blocks) 
## $UNDEAD performance analysis, 2025-06-28 

* "δ" indicates change since 2025-06-09 
* "α" is annualized since 2025-06-09 

![$UNDEAD rank](../05/imgs/snapshot/01a-rank.png) 
![$UNDEAD quote](../05/imgs/snapshot/01b-quote.png) 
![$UNDEAD market captalization](../05/imgs/snapshot/01c-cap.png) 
![$UNDEAD 24-hour volume](../05/imgs/snapshot/01d-vol.png) 

* rank: 8065 (δ: -4.33% ) , α: -83.25% 
* quote: $0.00226 (δ: -19.91% ) , α: -382.44% 
* market cap: $33,916 (δ: -20.75% ) , α: -398.67% 
* 24-hr volume: $110,772 (δ: -51.72% ) , α: -993.55% 

[2025-06-09 $UNDEAD report (archived)](https://github.com/pivoteur/biz/tree/main/blog/2025/06/05) 

# Liquidity Pools

Okay, this is the part where I talk about $UNDEAD liquidity pools (LPs). I do have LPs on @Uniswap, ...

![UNDEAD LPs on Uniswap](imgs/02a-uniswap-v4-lps.png)

... and can swap $UNDEAD on there, however, there's a problem: @KyberNetwork does not recognize Uniswap v4 pools, ...

![UNDEAD Uniswap LPs do not show on Kyber (because they are v4?)](imgs/02b-not-on-kyber.png)

... even though other DEX (e.g.: VeraSwap) do!

![VeraSwap natively accepts all Uniswap LPs](imgs/02c-but-on-veraswap.png)

I close one v4 pool, swap the pair to $ETH, and go to set up the v3 pool

![Close v4 LP](imgs/03a-close-v4-lp.png)
![Swap pair to $ETH](imgs/03b-swap-to-eth.png)

And this is why I hate @ethereum.

The v4 pools are structured so you don't pay a criminal amount of money in transaction fees.

The v3 pools? Not so much. It's gone up to $36 to establish a v3 pool, ... during no traffic.

What the actual ...?

![Select v3](imgs/04a-select-v3.png)
![Choose assets](imgs/04b-choose-assets.png)
![Provide Liquidity](imgs/04c-provide-liquidity.png)
![Doz transaction fees, doe](imgs/04d-criminal-transaction-fees.png)

Ah, well.

* When life hands you lemons, you make lemonaide.
* When @ethereum hands you high transaction fees, you select `cancel`.

Moving on.

### Providing Liquidity to Avalanche Uniswap LP

Instead of creating an Uniswap v3 @ethereum LP, I create an Uniswap v3 @avax LP: LP AVAX/UNDEAD.

![Bridging $AVAX-liquidity to Avalanche](imgs/05a-bridge-avax.png)
![Reasonable Transaction Fee](imgs/05b-tx-fee.png)

As $UNDEAD has no price-point on @avax, I set it manually, then provide $AVAX and $UNDEAD liquidity. 

![I manually set the UNDEAD/AVAX price-point for the LP](imgs/05c-set-price.png)
![Provide Liquidity to LP AVAX/UNDEAD on Avalanche](imgs/05d-provide-liquidity.png)

