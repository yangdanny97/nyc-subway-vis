# nyc-subway-vis
EDA + visualization of subway access/redundancy across neighborhoods in NYC

Analysis is done at the level of Neighborhood Tabulation Area (NTA). 

For each NTA, we can derive:
- number of subway stations within boundaries
- number of subway services w/ at least one station within boundaries
- number of other NTAs reachable via single seat subway ride (no transfers)
- number of other NTAs reachable via single transfer subway ride

The latter two use a graph based analysis, which could be used in the future to analyze redundancy or bottlenecks, or to identify the impact of shutting a particular line/bridge/tunnel down.

Limitations/known flaws:
- the two branches of the A are not differentiated
- the three different S are omitted
- PATH, LIRR, Metro North are not included, this analysis is subway only

Data from NYC and NY Open Data:
- [2020 NTA](https://data.cityofnewyork.us/City-Government/2020-Neighborhood-Tabulation-Areas-NTAs-Tabular/9nt8-h7nd/about_data)
- [Subway Lines](https://data.cityofnewyork.us/Transportation/Subway-Lines/3qz8-muuu)
- [Subway Stations](https://data.ny.gov/Transportation/MTA-Subway-Stations/39hk-dx4f/about_data)


