# Testing and Code Coverage

Hwæt, pivoteurs!

![Pivot protocol testing](imgs/01a-tests.png)
![Code coverage](imgs/01b-coverage.png)

Automation work proceeding apace. We're increasing our testing and 
code-coverage as we develop automation. 

# PIVOTS

![`dusk` report](imgs/02-dusk.png)

`dusk` calls for 4 close pivots. Let's examine some of them (the ones we can 
get to), starting with the largest volume pivots first. 

## UNDEAD-on-AVAX

Pivot #1, from 195 $AVAX to $UNDEAD doesn't meet the 10% gain-cut, so we move 
onto the next pivot.

![Trade slippage](imgs/03-slippage.png)

Maybe slippage or maybe price-movement invalidated this pivot. I don't know. 

## UNDEAD+USDC

![`dusk` ix 3 call](imgs/04a-dusk.png)
![Close UNDEAD-on-USDC pivot](imgs/04b-close-undead-on-usdc-pivot.png)

The next pivot (ix 3) the swap does surpass the 10% gain requirement, so I 
close this pivot.

![`wyrd`](imgs/04c-wyrd.png)

I enter the data into `wyrd` to close the pivot, but it does not process 
numbers with commas.

![`wyrd` errors out](imgs/04d-err-out.png)

This is a work in progress. 

### `wyrd` hot-fix

A hot-fix in just before 8 pm ET (that is: UTC midnight), allows `wyrd` to 
process the transaction correctly.

![`wyrd` hot-fix](imgs/05-hot-fix.png)

I enter this row into the UNDEAD+USDC close pivot table. 

*whew!*

## Open UNDEAD+USDC pivots 

![UNDEAD+USDC Ratio](imgs/07a-ratio.png) 
![Middling δ](imgs/07b-delta.png) 

The meh δ makes no call, but I open an UNDEAD-on-USDC pivot, anyway. 

![Open UNDEAD pivot](imgs/07c-open-undead-pivot.png) 

All UNDEAD+USDC assets are now committed to pivots. 



















The UNDEAD+USDC pivot pool composition and γ-apportionment are as charted. 

![The UNDEAD+USDC pivot pool composition](imgs/08a-comp.png) 
![The UNDEAD+USDC pivot pool γ-apportionment](imgs/08b-apport.png) 

