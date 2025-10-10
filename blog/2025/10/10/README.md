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
