# Working session, 2025-01-29

## Popeyes take-out

* Working on a structure to generalize each pool-page, because, let's face it, all the pool pages are exactly the same, that is: they display the same charts for their individual pools. Wouldn't it be nice to templatize a page and generate a specific page for that pool, based upon parameters.
* This is easier said than done, not so much for each pool page, but for the pools index page, as well, because that involves generating indices to these template-generated pages, ... that's easy enough, ... but then generating the HTML-content in an XSS-safe-way, then inserting that content into the DOM is a whole lot more work than I anticipated, facing it for the first time, although, I'm sure, once I get the first one down and correct, the others will fall in naturally, ...
* ... but then there's the identifying what 'this page' is in the context of the pool being displayed onto the page generated. How do I know what 'this page' isfrom the template's perspective, and this involves passing around variable and being aware of those variables from both the generatOR's perspective and from the generatED perspective.

sigh

This is a whole lot of infrastructure-work. I hate infrastructure work, as it, if done correctly, shows no change from the UX but fundamentally changes the infrastructure (that is: simplifies the developer's work). So, yes, 'simplified workflow' is 'good,' but at the cost of a lot of work that goes into simplifying that workflow.

It can't be helped, as the cost of complexity is now causing UX-failure as demonstrated by including Venn Diagramming has now broken the bar chart display (again).
