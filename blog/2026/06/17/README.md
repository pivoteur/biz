# Dividends and Reinvestments

Hwæt, pivoteurs.

Today @ParisBrand32180 and I were going to close an $UNDEAD pivot, but first 
I have to pay or reinvest yields to the investors for the previous two close 
pivots. I'll be working on that today.

Also, as I'm going about this process of paying and reinvesting yields, I'll 
be looking at automation here to make this process seemless.

## Workflow

Let's look at each close pivot in turn.

![UNDEAD-on-BTC close pivot](imgs/01-close.png)

Firstly, for the UNDEAD-on-BTC close pivot on 2026-06-11, we have a program 
that makes an entry into the close pivot table. That's called 
[`wyrd`](https://github.com/pivoteur/protocol/tree/main/dapps/wyrd), which 
works with 
[`appender`](https://github.com/pivoteur/protocol/tree/main/dapps/appender).

