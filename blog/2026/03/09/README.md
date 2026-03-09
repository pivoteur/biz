# Automation

G'day, pivoteurs

Our developer, @ParisBrand32180, is knocking down the dominos to protocol 
automation.

![Automation progress: simple automations working on 
a schedule](imgs/01-automation.png)

* `Scheduled Workflow` was our first test to see if we could activate autmation 
(we did).
* `coffee` is a test that we can schedule a daily automation (we can).

# `virtsz`

I've added an incremental improvement to `virtsz`: the dapp that identifies 
assets in virtual pivots.

The old version of `virtsz` (version 1.02) misidentified some assets as 
virtual that used $UNDEAD as seed.

![Old version of `virtsz` mislabeled some assets as 
virtual](imgs/02a-virtsz.png)

The new version (1.03) correctly excludes those assets from the report.

![New version of `virtsz`](imgs/02b-virtsz.png)

