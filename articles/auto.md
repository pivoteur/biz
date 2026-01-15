# Pivot Protocol Automation Update

tl;dr: The Pivot Protocol automation is coming along nicely, delivering a smooth
experience to investors and a streamlined workflow for operations and
maintenance. There is still much work to be done, but the protocol is shaping
up for a production release.

-----

The Pivot protocol is moving from its pre-release α stage of prove the 
mathematics work in real time in the markets to a β release where the 
rough-edges of the protocol, operated entirely manually, will be replaced by
automation, tested under load and verified for accuracy.

Pivot Protocol automation is divided into two camps:

1. User-facing experiences, such as staking (aka 'delegating'), unstaking, 
collecting yields, and reinvesting dividends. Before all these operations were
calculated manually and handled peer-to-peer. Going forward, in partnership
with Wagyu Games, the UX/user-experience will handle all these operations
automatically. The UX will also provide that standard protocol metrics, such
as TVL, ROI, APR, and staking amounts for protocol users. These automations
will be covered in another article when the β release goes live.

2. Backend operations, such as opening pivots, closing pivots, distributing
gains, and asset-management will be handled jointly by a set of dapps developed
in-house and by the UX, a wallet dapp.

Let's look at the progress made by the backend dapps, most recent developments
first.

## Open Pivot dapps

### `virtsz`

![Virtual pivot assets](imgs/auto/01-virtsz.png)

First up, we have `virtsz`. `virtsz` calculates the assets committed to 
virtual pivots.

Why is this useful?

If there are pivots 'stuck' at an ATH or ATL price-ratio for assets in a pivot
pool and these pivots are virtual, then, upon analysis, we can simply pretend
these pivots do not exist (anymore). What does that do for us? It frees these
assets stuck in pivots that would require a massive market-swing for a 
close-pivot call. These freed assets can be allocated to new pivots in the
current market range, opening up possibilities for pivot-gains sooner.

### `assets`

![Pivot pool assets](imgs/auto/02-assets.png)

`assets` provides a snapshot of all pivot pool assets, providing also each
pivot pool's TVL. What does this do for operations?

It shows me the relative strength of each pool which comes into play in
deciding which pools to axe or to reinforce and which pools are full steam
ahead and good to go.

### `dawn` [WIP]

The above two dapps, combined with some elbow-grease, ... and adding some
blood, sweat, and tears, will produce `dawn` when reviews all pivot pools'
assets and determines which pools on which to open pivots, and in which
directions to open those pivots.

## Close Pivot dapp

### `dusk`

How is automation helping? `dusk` is the answer.

Before I would work 20 hours each day to collate data to compute which pivots
to close onto which pivot pools, and do other operations and maintenance work
as well as development work for the protocol.

![`dusk` report of close pivots](imgs/auto/03-dusk.png)

`dusk` now goes through every pivot pool and, based off market prices for the
day, computes which pivots to close at what rates of return.

This automation, alone, saved me 8 hours each day, reducing my work-day to a
more-reasonable 12-hour work-day.

Not only that, but since `dusk` has become operational I am closing (and then
consequently) opening more pivots each day, returning more gains to the
protocol investors.

Efficiency: it pays off.

-----

The [Pivot Protocol](https://pivoteur.github.io/#) is currently in pre-release
α with a β release this month. We're looking to go into full production release
in the first half of this year, 2026.
