# 2025-06-17 Status of $UNDEAD 

![$UNDEAD rank](imgs/01a-rank.png) 
![$UNDEAD quote](imgs/01b-quote.png) 
![$UNDEAD market captalization](imgs/01c-cap.png) 
![$UNDEAD 24-hour volume](imgs/01d-vol.png) 

* rank: 7860 
* quote: $0.00271 
* market cap: $40,607 
* 24-hr volume: $238,178 (δ: -$2,904 ) 

When we get LPs funded on multiple blockchains, what will $UNDEAD look like? 

[$UNDEAD data source](https://www.coingecko.com/en/coins/undead-blocks) 
## $UNDEAD performance analysis, 2025-06-17 

* "δ" indicates change since 2025-06-05 
* "a" is annualized since 2025-06-05 

![$UNDEAD rank](../05/imgs/snapshot/01a-rank.png) 
![$UNDEAD quote](../05/imgs/snapshot/01b-quote.png) 
![$UNDEAD market captalization](../05/imgs/snapshot/01c-cap.png) 
![$UNDEAD 24-hour volume](../05/imgs/snapshot/01d-vol.png) 

* rank: 7860 (δ: -4.13% ) , a: -125.73% 
* quote: $0.00271 (δ: -10.54% ) , a: -320.65% 
* market cap: $40,607 (δ: -10.54% ) , a: -320.61% 
* 24-hr volume: $238,178 (δ: 48.23% ) , a: 1466.95% 

[2025-06-05 $UNDEAD report (archived)](https://github.com/pivoteur/biz/tree/main/blog/2025/06/05) 

# PIVOTS 

## ETH+UNDEAD 

No close pivots. 

The positive δ calls to open an ETH-on-UNDEAD pivot, which I do. 

![Positive δ](imgs/02a-pos.png) 
![Open ETH pivot](imgs/02b-open-eth-pivot.png) 

The Echo pool composition and γ-apportionment are as charted. 

![Echo pool composition](imgs/03a-comp.png) 
![Echo pool γ-apportionment](imgs/03b-apport.png) 

## UNDEAD+USDC

Now, yesterday, I said I was going to open an UNDEAD+USDt pivot pool, however, @Uniswap had no trading path for that for a while.

![No USDt-to-UNDEAD swap on Uniswap](imgs/04-usdt.png)

That seems to have cleared up.

At any rate, I'm going with an UNDEAD+USDC pivot pool, as USDC seems to be more widely accepted.

So, I move some $ETH and some reserve $UNDEAD from the Echo pool to the new UNDEAD+USDC pivot pool. 

![Transfer ETH (gas)](imgs/05a-xfer-eth.png)
![Transfer reserve UNDEAD](imgs/05b-xfer-undead.png)

This requires I reconfigure my Echo pool γ-factors and configure new γ-factors for the UNDEAD+USDC pool. 

![Reconfigure Echo pool γ-factors](imgs/05c-reconfigure-echo.png)
![Configure UNDEAD+USDC γ-factors](imgs/05d-configure.png)

Even though the new pool has all $UNDEAD, I'm pretending a 50/50 split.

UNDEAD+USDC

This is a new pivot pool.

![Negative δ](imgs/06a-neg.png)

The negative δ calls to open an USDC-on-UNDEAD pivot, which I do. I also establish a hedge by opening an UNDEAD-on-USDC pivot.

![Open USDC pivot](imgs/06b-open-usdc-pivot.png)
![Open UNDEAD hedge](imgs/06c-open-undead-hedge.png)

And thus we have a new pivot pool with its first pivot and hedge.

The UNDEAD+USDC pivot pool composition and γ-apportionment are as charted.

![UNDEAD+USDC pivot pool composition](imgs/07a-comp.png)
![UNDEAD+USDC pivot pool γ-apportionment](imgs/07b-apport.png)


# Providing Liquidity on Uniswap 

I provide 100k $UNDEAD and an equivalent amount of the pair for 
both the ETH/UNDEAD LP and the UNDEAD/USDC LP on Uniswap. 

![Swap UNDEAD to ETH](imgs/08a-swap-to-eth.png) 
![Swap UNDEAD to USDC](imgs/08b-swap-to-usdc.png) 

Creating a Liquidity pool on @Uniswap is as easy as can be:

* I choose 'create new pool.'
* I select the pair and set fees to 1% for this exotic pool
* I provide the liquidity
* ... and now I have a liquidity pool on Uniswap!

![Create Pool on Uniswap](imgs/09a-create-pool.png)
![Provide pair liquidity](imgs/09b-provide.png)
![My pool-list](imgs/09c-list.png)
![Pool Details](imgs/09d-details.png)

I follow the same steps to provide liquidity to the newly-created ETH/UNDEAD LP on @Uniswap.

![Create Pool on Uniswap](imgs/10a-create-pool.png)
![Provide pair liquidity](imgs/10b-provide.png)
![My pool-list](imgs/10c-list.png)
![Pool Details](imgs/10d-details.png)

# CONCLUSION 

This concludes pivot-activity for today. 

![Pivot Protocol dashboard](imgs/11a-dash.png) 
![Pivot Protocol TVL](imgs/11b-tvl.png) 

[The Pivot protocol](https://pivoteur.github.io/#) 
