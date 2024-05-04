# nyc-subway-vis
EDA + visualization of subway access/redundancy across neighborhoods in NYC.

Analysis is done at the level of Neighborhood Tabulation Area (NTA). 

For each NTA, we can derive:
- number of subway stations within boundaries
- number of subway services w/ at least one station within boundaries
- number of other NTAs reachable via single seat subway ride (no transfers)
- number of other NTAs reachable via single transfer subway ride

The latter two use a graph based analysis, which could have other interesting applications in this space.

Notes:

- the two branches of the A are not differentiated
- only the Franklin Ave S is included
- SIR is omitted since it's not connected with the rest of the subway system
- only daytime routes are considered - no rush hour/nighttime service changes

Data from NYC and NY Open Data:
- [2020 NTAs](https://data.cityofnewyork.us/City-Government/2020-Neighborhood-Tabulation-Areas-NTAs-Tabular/9nt8-h7nd/about_data)
- [Subway Lines](https://data.cityofnewyork.us/Transportation/Subway-Lines/3qz8-muuu)
- [Subway Stations](https://data.ny.gov/Transportation/MTA-Subway-Stations/39hk-dx4f/about_data)

Ideas for Future:

- a graph-based approach could be used in the future to analyze redundancy or bottlenecks, or to identify the impact of shutting a particular line/bridge/tunnel down
- visualizing this by census tracts is more practically useful than NTA due to higher granularity
- use distance-based calculations instead of neighborhood boundaries, since some stations lie right outside an NTA and some larger NTAs contain areas that aren't reachable by train
- instead of just counting the number of reachable neighborhoods, another metric to consider might be the total population in the reachable neighborhoods


