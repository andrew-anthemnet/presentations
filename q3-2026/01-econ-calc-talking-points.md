# Talking Points — Econ Calculator

--- 
## Opening — The Problem

### Why we built this
Today, developing a site-level pro forma is a significant manual effort. Every site requires someone to pull numbers from QuickBooks, reference SiteTracker, apply the lease terms, factor in construction costs, and assemble it all in a spreadsheet. That takes time, and the moment it's finished, it's already at risk of being out of date.

If a lease gets executed this afternoon and we now have certain ground rent terms — that pro forma from this morning doesn't reflect it. If we need to model a different tower type, someone has to rebuild the analysis. And because these live in individual files, there's no consistency in how they're structured, no standard set of assumptions, and no easy way to tell where a particular number came from or how much confidence we should have in it.

The deeper issue is that we have no persistent, reliable view of a site's financial picture as it moves through its lifecycle. We get snapshots — accurate for a moment, then stale — and we make decisions from them anyway because there's no alternative.

--- 

### Introduce — What Tower Finance Is
The econ calculator is a web application purpose-built for Anthemnet that gives everyone a self-serve, living, always-current pro forma for every site in our portfolio. You log in, pick a site, and you're looking at a full financial picture — revenue by carrier, ground lease costs, development and construction spend, operating expenses, net cash flow — all of it structured the same way, every time, for every site. Built on top of that is a financial health framework that makes up what we have been talking about as our "Econ Calculator". This is a set of criteria to assess each sites financial standing at any point in our process.

The application gets more accurate as the site progresses. Every piece of data in the system has a trust level that is visually shown. A seeded default is the lowest — it's our best guess. A SiteTracker value is more certain — someone entered it from a real document. A QuickBooks actual is near the top — it's a real financial transaction. As the site progresses and we enter data into SiteTracker and record transactions in QuickBooks, the pro forma automatically layers in our most certain information over our initial estimates. 

___ 

### Other Capabilities 
Other capabilites in this system is a construction costs test bench to let you see how different tower attributes effect construction costs to help in early stages of the site development. This system exposes every driver that a site's finances depend on and lets you adjust them.

Layered onto this will be a financial health framework — a set of criteria we define to assess each site's financial standing. Are development and construction costs within expected ranges? Are we seeing large deviations from our budgets or estimates? Are the lease terms yielding the returns we projected? The system will surface these automatically so we're not waiting for a review to discover a site is trending in the wrong direction.

Longer term, the algorithms and data behind Tower Finance feed into many more systems. Site reviews. Lease negotiation. Budgeting. Portfolio-level analysis. This is the foundation — the financial intelligence layer that everything else can draw from.

___ 

### Close — Timeline

I'll be releasing Tower Finance and going live over the next couple of weeks. During that window I'll be doing hands-on testing with each of you — walking through real sites, validating the numbers, and making sure the tool fits how you actually work. Your feedback during that period is critical. This was built to solve a real problem in how we manage site economics, and getting it right means getting your input on the details.
