# Workers' Compensation Loss Reserving with the Chain Ladder Method

## The question
How much did a workers' compensation insurer still owe on claims that had already happened as of the end of 2007?

## The data
Real insurer data from the CAS Loss Reserving Database, which comes from the Schedule P section of the annual statements insurers file with regulators. I used one company, Beacons Mutual Insurance Company, with accident years 1998 through 2007. Amounts are cumulative paid losses in thousands of dollars.

## What I did
I built a paid loss triangle in Excel using only data available at the end of 2007. From it I calculated age to age factors showing how much each accident year's payments grew from one year to the next, then selected volume weighted average factors so larger years carried more weight. I chained those into cumulative development factors, projected each accident year to its ultimate loss, and subtracted what had already been paid to get the reserve. I assumed no development after year ten.

## Results
The estimated total reserve at the end of 2007 is about $146.5 million. Most of it comes from the newest accident years, with 2005 through 2007 making up about $121.7 million, since those claims were still early in their payout.

I then compared my projected ultimates to the actual amounts paid through year ten. The older accident years came within 1 percent, while the newest years were off by as much as 12 percent. That makes sense, because a large development factor multiplies any unusual movement in a single early data point.

Overall the method estimated a reserve of about $146.5 million compared to an actual of about $122.3 million, an overestimate of roughly 20 percent. Every recent accident year was overestimated, which suggests newer years developed more slowly than older years did.

## Limitations and next steps
Assuming no payments after year ten likely understates the reserve, since workers' comp claims can pay out for a very long time, so a tail factor would be the next improvement. Since the comparison to actual also stops at year ten, the overestimate above is a fair like for like result, but the true ultimate reserve would be somewhat higher than both figures. I would also try the Bornhuetter Ferguson method, which leans on expected losses for the newest years instead of relying only on one early data point, and compare the results to a chain ladder on incurred losses.

## Files
loss_reserving_chain_ladder.xlsx contains the triangle, development factors, reserve summary, and comparison chart.
