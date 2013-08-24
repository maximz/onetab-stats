onetab-stats
============

Compute and visualize statistics about your browsing patterns using data from the OneTab Chrome extension.


### Goals

**Initial sections:**

* Parsing
* Global histogram (how many tab group creations on each day in this 4 month span)
* Time of day: global histogram, May histogram, June histogram, July histogram, August histogram of tab group creation (bin by hour - i.e. create a new column named hourNumber, extract hour number from the time string, and place it in that column, then run hist() on that column)

**Todo:** not just how many tab groups, but how many tabs were visited on each day in this 4 month span AND histogram of number of tabs visited at different times of day in each month and globally

**Coming soon:** URL metadata. i.e.:

* which domains are the most visited (histogram of domain visited count based on which day in the 4-month period, and which time of day (globally and by month))
* then find a way to assign one of three classes to each domain: {educational, entertainment, work} - and see all those graphs in above bullet with data binned into these three classes.

**Way down the road:**

Build a Chrome extension that keeps track of all tabs you open, not just the ones you choose to save (i.e. the OneTab model). Then, we produce the equivalent of the account usage summary reports Google churns your GPS logs into.

This will all happen client side, of course; the Google Chart API can handle our pie-charting needs, but is their a good way to create histograms in JS?
