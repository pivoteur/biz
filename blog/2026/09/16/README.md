# `hwaet`

HWÆT, pivoteurs, and well-met!

![Automation shows `hwaet` failure](imgs/01a-actions.png)
![ `hwaet` debug run](imgs/01b-hwaet.png)
![Protocol dashboard](imgs/01c-diag.png)
![BTC+ETH pivot pool overcommitted](imgs/01d-btc-eth.png)

Automation this morning shows a `hwaet` (pool health) failure. I dug into this 
and it shows I've overcommitted 0.37 BTC into pivots.

Why? An investor withdrew as much, and I accounted for this after I pivoting.

No problem. I'll adjust pivots now.

## Adjustment

After adjusting the pivots, `hwaet` now runs successfully.

![ `hwaet` run](imgs/02a-hwaet.png)
![BTC+ETH liquidity 'discovered'](imgs/02b-btc-eth.png)

Not only that, but $3,900 of BTC-liquidity is 'discovered' in the 
adjustment-process, which is cool!

Let's pivot that liquidity with automations to do that ([issue to create 
automations](https://github.com/pivoteur/trading/issues/88)).

# Pivots and (building) automation

## `frignan`

The first automation is

![ `frignan` ](imgs/03a-frignan.png)
![BTC quote](imgs/03b-btc.png)

* [ `frignan` ](https://github.com/pivoteur/trading/actions/workflows/frignan.yml)

which queries the blockchain for the current price of an asset.

## `gelic`

Next, let's create automation for

![ `gelic` run](imgs/04a-gelic.png)
![wallet balance on Avalanche](imgs/04b-balance.png)

* [ `gelic` ](https://github.com/pivoteur/trading/actions/workflows/gelic.yml)

which reads a wallet's balances on a blockchain.

You see this wallet is empty, so we'll need to provide liquidity (with the 
next dapp).

