G'day, pivoteurs! 2025-10-10

Another speed-run today? Nupe!

Today, I'm not doing the 50'-sprint. Today, we're doing the Marathon:

* All pivot pools, all pivot-actions, including:

1. close pivots
2. distributions
3. open pivots
4. assessments

Let's go.

# bae

## price-quote data collection

Before I do pivots, I get price-quotes from around the Blockaverse.

I use my Rust-app: bae

![`./bae`](imgs/01a-bae.png)

This quote-collection automation saves me hours per day from before!

![Archive all quotes](imgs/01b-quotes-all.png)
![Collate protocol quote](imgs/01c-quotes-protocol.png)
![Update spreadsheet](imgs/01d-spreadsheet.png)

Collating these quotes into the protocol for analysis is still a manual process, relying on 12 spreadsheets.

# UNDEAD

![UNDEAD stats on coingecko](imgs/02a-undead.png)

Next up, I collect data specifically on the $UNDEAD-token. I collect:

* rank
* price
* market cap
* 24-hour volume

Then update my spreadsheet with these values. 

![Update spreadsheet](imgs/02b-update.png)

This process is 100% manual, but the data quality is unique.

I have collected these metrics for over 300 days.

## Git-as-database

I don't just hold these data locally. I move all data collated to git as TSV-files.

![Copy data from spreadsheet](imgs/03a-copy.png)
![Paste data into repository](imgs/03b-paste.png)
![Data visualization on spreadsheet](imgs/03c-spreadsheet.png)
![Update git](imgs/03d-git.png)

Primitive database? You betcha.<br/>
Does it work? For now.

Should I use cloud databases and automated integration? Absolutely!

"Some day"* I'll do that.

* some day, n. indef.: ... when I have time

# Protocol metrics

"Does it work?"

What even does that mean, in light of all this time and effort? 

The payoff for me, and the protocol's stakers, is we have up-to-date metrics on the pivot pools, the protocol, and the $UNDEAD-token. 

![Protocol dashboard](imgs/04a-dash.png)
![UNDEAD chart](imgs/04b-undead.png)
![UNDEAD report](imgs/04c-undead-report.png)
![Pivot pools](imgs/04d-pools.png)

# Other Protocol Housekeeping

Does that mean we're ready to pivot?

Not yet.

I have a spreadsheet that guides my work:


1. DEX-race.

![DEX-race template](imgs/05a-spr-dex.png)

2. LPs

![LPs template](imgs/05b-spr-lps.png)

3. BTC Vault

![BTC vault template](imgs/05c-spr-btc.png)

4. ... THEN pivoting.

Let's go.
# DEX UNDEAD/USDC-swap Race 

Same swap; 3 DEX, 2025-10-10 

I swap 202000 $UNDEAD for: 

1. 476.59 $USDC on @BlackholeDex 

![UNDEAD/USDC swap on Blackhole](imgs/06a-blackhole.png) 

2. 514.55 $USDC on @KyberNetwork 💥 

![UNDEAD/USDC swap on Kyber](imgs/06b-kyber.png) 

3. 514.55 $USDC on @LFJ_gg 💥 

![UNDEAD/USDC swap on LFJ](imgs/06c-lfj.png) 

TIE! between @KyberNetwork and @LFJ_gg 

# Liquidity Pools 

## Liquidity Pool Positions 

![Blackhole UNDEAD LPs](imgs/07a-blackhole-lps.png) 
![Uniswap UNDEAD LPs](imgs/07b-uniswap-lps.png) 

The Blackhole and Uniswap $UNDEAD LPs are as shown. 

# Bitcoin vault 

* I swap some accumulated $AVAX to $BTC.b 

![Swap to $BTC](imgs/08a-swap.png) 

* I send this $BTC.b to the vault 

![Send BTC to vault](imgs/08b-sned.png) 

# Tether

![Price spike on $USDt](imgs/09-usdt.png)

Did somebody instigate a run on $USDt? #Tether 

# PIVOTS 

## BTC+ETH 

![Close ETH-on-BTC pivots](imgs/10a-close-eth-on-btc-pivot.png) 

I close 7 ETH-on-BTC pivots for gains of: 


* actual ROI: 15.39% / 117.05% APR projected 
* or: 2.50 $ETH -> $BTC -> 2.88 $ETH 
* or: $1,462.71 gain on 7 pivots totalling $10,924.44 


![Distribute gains to stakers](imgs/10b-dist-gains.png) 

I reinvest the gains or distribute 80% to stakers. 



... and that --^ is how to PROFIT ~$1.5k during a turbulent market. 

## Open BTC+ETH pivots 

![BTC+ETH Ratio](imgs/11a-ratio.png) 
![Positive δ](imgs/11b-delta.png) 

The positive δ calls to open an BTC-on-ETH pivot, which I do. 

![Open BTC pivot](imgs/11c-open-btc-pivot.png) 

I also open an ETH-on-BTC hedge. 

![Open ETH hedge](imgs/11d-open-eth-hedge.png) 





The BTC+ETH pivot pool composition and γ-apportionment are as charted. 

![The BTC+ETH pivot pool composition](imgs/12a-comp.png) 
![The BTC+ETH pivot pool γ-apportionment](imgs/12b-apport.png) 

