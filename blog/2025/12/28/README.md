# PIVOTS

![`dusk`-report](imgs/01-dusk.png)

`dusk` reports no close pivots today, but also ... 

... `dusk` is not able to handle synthetic nor wrapped tokens. 

![`dusk` needs token-aliasing](imgs/02-aliases.png)

So: I need to backpropagate aliases from `assets` to `dusk`. 

# TODOs

* continue working on open-pivot automation
* relocate assets from @avax to @hedera 

and:

![AVAX/HBAR ratio](imgs/03a-avax-hbar.png)
![BTC/AVAX ratio](imgs/03b-btc-avax.png)
![BTC/HBAR ratio](imgs/03c-btc-hbar.png)

There may be a way to transliterate BTC+AVAX to BTC+HBAR if $AVAX and $HBAR 
share ratio-characteristics when the pivots were opened: I'll investigate this 
possibility.

# AUTOMATION ANNOUNCEMENT

I've released a new revision of 
[`dusk`](https://github.com/pivoteur/protocol/tree/main/dapps/dusk), 
version 1.08:

![`dusk` revision compacting report and handling wrapped tokens and 
synthetics](imgs/04-dusk-revision.png)

* it now aliases tokens, meaning that it handles synthetics and wrapped tokens
* it compacts no-close-calls pivot pools, reducing the size of the report. 

