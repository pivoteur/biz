# dapp failures

HWÆT, pivoteurs, and well-met!

![Protocol health: dapp failures](imgs/01-health.png)

We have a couple of failures of protocol dapps: hwaet and dusk. Let's take a 
look-see what happened.

## `dusk`

![ `dusk` run](imgs/02a-dusk.png)
![BTC+ETH pool removed](imgs/02b-btc-eth.png)

For `dusk`, the error was 'empty list for data-set.' Looking at the data-sets 
updated last night, I see that the BTC+ETH pool has been wiped out.

I'll restore that pool's data (I have a local back-up), and see if that fixes 
the problem.

