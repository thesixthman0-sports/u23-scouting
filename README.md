# Scouting by the Numbers: Under-23 Players in Europe's Top Four Leagues, 2015/16, and What Happened Next

Which young players stood out statistically at their position in 2015/16, and what became of them?
I ranked players with the metrics scouts typically use for each position, picked the best under-23s
using rules fixed in advance, and only then looked at their careers.

*Second project in a series. First project: [Finding Similar Players: a Serie A 2015/16 case study](https://github.com/thesixthman0-sports/scout-analytics-football).*

## Summary

- Event data (StatsBomb, 1,517 matches) for **1,251 outfield players and 101 goalkeepers** with 900+ minutes in the
  Premier League, La Liga, Serie A and Ligue 1, linked to Transfermarkt career data.
- Players were compared with **all players of the same role** (percentiles), using 6–7 position-specific metrics.
- **Nobody under 23 stood out clearly** (average percentile of 85+ in the role). The best reached 80. Even across all
  ages only 7 players reached 85 (Neymar, Messi, Marcelo, Alexis Sánchez, Modrić, Coquelin, Verratti).
- I followed the 22 best outfield players under 23 (and the 3 best young goalkeepers). **Careers split widely:**
  Dembélé, Sterling, Dybala, Marquinhos and Umtiti became very valuable; Cabot, Sylla and Juncà never went beyond a few million.
- **Compared with other young regular starters, the selected players reached higher peak values (82% vs 57% above
  €20M, p = 0.046), but this largely reflects higher starting prices.** After controlling for starting value, age and position,
  I find no clear advantage (+10% growth by 2019, 95% CI −27% to +67%), and they were no more likely to keep playing in the top
  leagues (82% in both groups).

## Data

- **StatsBomb Open Data:** Serie A, Premier League, La Liga and Ligue 1, 2015/16 (1,517 matches; Ligue 1 has 377 of 380).
- **Transfermarkt**, via the open dataset [transfermarkt-datasets](https://github.com/dcaribou/transfermarkt-datasets)
  (CC0): market-value history to June 2026, birth dates, appearances and career status.
- **Linking the sources:** names differ across sources (nicknames, accents), so players were matched by name within their
  club, and every link was checked against minutes played in Transfermarkt's appearance table (ratio to StatsBomb minutes:
  mean 0.96, SD 0.02). 1,233 of 1,251 outfield players and 99 of 101 goalkeepers were linked. Age is age on 30 June 2016.

## Method

1. **Per-90 metrics** from event data. Percentage metrics (tackle success, aerial duels won, pass completion
   under pressure, npxG per shot) were shrunk toward the role average using 5–30 pseudo-attempts, so that 3 wins
   out of 3 does not count as 100%.
2. **Possession adjustment:** defensive actions are scaled by team possession (share of passes in the team's matches),
   using a power chosen so that possession no longer correlates with players' defensive workload (r = −0.04).
3. **Metrics by role**, chosen from published scouting and recruitment material before
