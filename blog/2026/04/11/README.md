# Automation

G'day, pivoteurs

Today we have 4 automations going, thanks to the research and development by 
@ParisBrand32180.

## `quotes`

First is `quotes`: it fetches the quotes daily and reposes them in github, so 
you can do your own analytics.

![`quotes`-automation](imgs/01a-quotes.png)
![Daily quotes](imgs/01b-quotes.png)

You can [use the reposed 
quotes](https://raw.githubusercontent.com/logicalgraphs/crypto-n-rust/refs/heads/main/data-files/csv/quotes.csv).

## Protocol O&M

The next three automations are related to protocol operations and maintenance. 

![Protocol O&M automations](imgs/02a-prot.png)
![Close pivot calls](imgs/02b-calls.png)

They are:

* `assets` that compute procotol asset TVLs
* `virtsz` that recomputes all virtual pivots; and,
* `dusk` that makes close pivot calls

Each component is building toward an automated protocol

