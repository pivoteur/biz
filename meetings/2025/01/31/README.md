# Working session, 2025-01-31

## McDonald's take-out

* Worked on gathering miscellaneous crypto of less than 5% of total value into an 'others'-category.
* This all would've been straightforward work if I weren't using Javascript, particularly with iterations over collections:

<code>for(let x in collection)</code>

gets you what? `x` isn't each element of the collection, no! `x` is, sequentially, 0, 1, 2, 3, ...

What the ever-loving what?

That took me all day of screaming at the charts: "WHY?" to find and to fix.

When I *did* find the issue, it was easily fixed, but Javascript's unique-take on things like totality and what is being iterated over and boolean values (which is a specialization of totality) and the very odd times it rears its inscrutable head is more than annoying: it's detrimental to progress.

* So, anyway: 'others'-category separately implemented for each of pie-charts and bar-charts. I'm not doing an 'others' for Venn Diagram, because that'd be beastly (what are the intersections to 'others,' pray, tell?) and, so far, the Venn diagram is clean, so we're good for now.
