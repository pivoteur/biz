# Working Session, 2025-02-05

## Chick-fil-a takeout

* Via experimentation, created a template-page of a (parameterized) pivot pool
* Created a function that generated the donor (wallet) address to stake to the pivot pool, ... this is more complicated than it sounds, as it requires creating a static function from asynchronous data. Via experimentation I was able to populate address data onto the page asynchronously THEN create the static function from that (now) established (that is: set) data. This process of setting state from asynchronous data is known as 'freezing.'
* Updated the pools-page's indices to point each pivot pool to this new template pivot pool page.
* Viewed results, tested all links to and from this template page in multiple instances
* deployed to production
* Removed seven static pool pages. Now only using the template page for pivot pools

* Saw that non-pivot pools (i.e.: the treasury and the echo pool) where not being handled correctly from the pools index page. Created an use case for non-pivot pools, implemented this solution, tested it, and rolled this correction out to production.
