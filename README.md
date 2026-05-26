# student-convexity-graph
Introductory graph to show differences in mod vs convex dv01

This was a simple project where I introduced the concept of Mod Durations vs Convexity in bond price for various rate shocks.

It was also the first excel where 100% of the process was done manually without ai, hence the ultra simplified UI.

The important concepts here are

Mod DV01
newPrice = 0Price(1-Dmod(bp/10,000))

Convex DV01
newPrice = 0Price(1-Dmod(bp/10,000)+.5*Convexity((bp/10,000)^2))

NOTE: This is pricing for a par of 100, the "10,000" variable can be adjusted


IMPORTANT OBSERVATIONS

While mod dv01 kept the hypothetical bonds price with a linear change per basis point, convexity increased dv01 exposure as rates fell and decreased dv01 as rates increased
This is significant as it gives the bond "cushion" on upwards rates and "leverage" as rates fall
Which is a concept that long duration PMs use to build exposure while minimizing downside
