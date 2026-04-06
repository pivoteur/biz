# Automation

G'day, pivoteurs!

![Automation](imgs/01-automation.png)

The automation-work done by @ParisBrand32180 has been extremely useful, but has 
also pointed out the need for even more automation.

Let's enumerate the immediate needs (🧵)

## `virtsz`

First off:

![Available assets](imgs/02-available.png)

* `virtsz` automatically adjusts virtual pivots, but it doesn't do anything 
with available assets in a pool. The next version needs to commit all 
available assets to virtual pivots, automatically. 

## `assets`

Secondly:

![`assets` and wallet totals](imgs/03-assets.png)

* `assets` automatically updates the TVLs of the protocols, but `assets` is 
based upon wallet-totals, which, themselves, are not automated.

Wallet totals simply sum the pivot pools and treasuries, so, in theory, should 
be easy enough to automate.

## `dusk`

Thirdly:

![`dusk`-report](imgs/04a-dusk.png)
![Close pivot still in process](imgs/04b-close.png)

* `dusk` makes identifying closing pivots much easier now, shaving hours off 
the process, but ...

Closing pivots entail a lot of infrastructure, including distributions and 
data-marshalling around the pools and profiles: I have a close pivot in process 
from March 31st.

Automation to help expedite close pivots:

* `distr` that distributes pivot-gains to investors
* `closr` marshals data around the closed pivot in three areas:

1. Create the close-pivot row (gains, ROI, APR)
2. Close the open-pivot(s) with the close-pivot ID
3. Update profiles

