# Scouting by the Numbers: Under-23 Players in Europe's Top Four Leagues, 2015/16, and What Happened Next

Which young players stood out statistically at their position in 2015/16, and what became of them?
I ranked players with the metrics scouts typically use for each position, picked the best under-23s
using rules fixed in advance, and only then looked at their careers.

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
3. **Metrics by role**, chosen from published scouting and recruitment material before looking at any result:

| Role | Metrics |
|---|---|
| Strikers | npxG/90, non-penalty shots/90, npxG per shot, touches in the box/90, xA/90, pressures/90 |
| Wingers / attacking midfielders | xA/90, key passes/90, npxG/90, touches in the box/90, progressive carries/90, dribbles won/90 |
| Central midfielders | progressive passes/90, pass completion, pass completion under pressure, xA/90, progressive carries/90, tackles + interceptions/90, ball recoveries/90 |
| Defensive midfielders | progressive passes/90, pass completion, pass completion under pressure, tackle success %, tackles + interceptions/90, recoveries/90, aerial duels won % |
| Full-backs | completed crosses/90, xA/90, progressive carries/90, progressive passes/90, tackle success %, tackles + interceptions/90 |
| Centre-backs | aerial duels won %, tackle success %, interceptions/90, clearances/90, progressive passes/90, pass completion, fouls (fewer is better) |

4. **Percentiles** within role among all 1,251 players; the role score is the mean percentile of its metrics.
5. **Selection rules, fixed before looking at outcomes:**
   - *Standout:* score of 85+ and at least 3 metrics at the 80th percentile or above.
   - *Fallback (because no young player qualified):* the 5 best under-23s in each group (attackers, midfielders,
     defenders) plus the 3 best in each of the six roles, 22 players in total. The "3 per role" extension was added after seeing
     the top-5 lists, which contained only statistics, and before looking at any value or career outcome.
   - Under 23 on 30 June 2016, 1,500+ minutes (101 players: 25 wingers/AM, 21 full-backs, 21 central midfielders,
     16 centre-backs, 11 strikers, 7 defensive midfielders). Goalkeepers: the 3 best under-23s with 1,500+ minutes.
6. **Outcomes, looked at last:** Transfermarkt value nearest 30 June 2017, 2018, 2019 and 2021, peak value and year, last
   season played, and minutes in the top-5 leagues in 2018/19 and 2019/20.

## Results

### 1. Who stands out

Sanity check of the ranking: the best players of all ages by role are the ones you would expect: Neymar (98) and Messi (96) among
wingers, Modrić (86) and Verratti (85) among central midfielders, Coquelin (86) among defensive midfielders, Marcelo (93) among
full-backs. The best strikers were Luis Suárez (81) and Gameiro (78), the best centre-backs van Dijk (76) and Mertesacker (76).
Among under-23s the top of each group is below the standout bar: Baldé 80, Dembélé 78, Tolisso 75, Rabiot 74, Sylla 77.

### 2. The 22 selected outfield players and what happened

Value in EUR millions (Transfermarkt, nearest to 30 June), peak value and year, and whether the player played 900+ minutes
in the top-5 leagues in 2018/19 or 2019/20.

| Role | Player (2015/16 team) | Age | Score | 2016 | 2018 | 2019 | Peak (year) | 900+ min, top-5 leagues 2018–20 |
|---|---|---|---|---|---|---|---|---|
| AM/W | Keita Baldé (Lazio) | 21 | 80 | 10.0 | 30.0 | 25.0 | 30.0 (2018) | no |
| AM/W | Ousmane Dembélé (Rennes) | 19 | 78 | 12.0 | 80.0 | 100.0 | 120.0 (2019) | yes |
| AM/W | Bruma (Real Sociedad) | 22 | 74 | 5.0 | 12.5 | 10.0 | 12.5 (2017) | no |
| AM/W | Raheem Sterling (Man City) | 22 | 73 | 45.0 | 90.0 | 140.0 | 160.0 (2019) | yes |
| AM/W | Anthony Martial (Man United) | 21 | 72 | 32.0 | 65.0 | 60.0 | 65.0 (2018) | yes |
| CM | Corentin Tolisso (Lyon) | 22 | 75 | 7.5 | 45.0 | 40.0 | 45.0 (2018) | no |
| CM | Adrien Rabiot (PSG) | 21 | 74 | 10.0 | 50.0 | 35.0 | 50.0 (2018) | yes |
| CM | Emre Can (Liverpool) | 22 | 70 | 18.0 | 30.0 | 40.0 | 40.0 (2019) | yes |
| CM | Jimmy Cabot (Troyes) | 22 | 65 | 1.5 | 1.5 | 1.0 | 5.0 (2022) | no |
| DM | Leandro Paredes (Empoli) | 22 | 64 | 6.0 | 20.0 | 35.0 | 40.0 (2019) | yes |
| DM | Amadou Diawara (Bologna) | 19 | 62 | 9.0 | 18.0 | 15.0 | 23.0 (2020) | yes |
| DM | Seko Fofana (Bastia) | 21 | 51 | 1.5 | 9.5 | 13.0 | 32.0 (2023) | yes |
| FB | Issiaga Sylla (Gazélec Ajaccio) | 22 | 77 | 2.0 | 3.0 | 3.5 | 3.5 (2019) | yes |
| FB | Benjamin Mendy (Marseille) | 22 | 74 | 6.5 | 40.0 | 35.0 | 45.0 (2018) | yes |
| FB | Ricardo Pereira (Nice) | 23 | 72 | 4.5 | 20.0 | 25.0 | 40.0 (2019) | yes |
| FB | David Juncà (Eibar) | 23 | 71 | 2.5 | 1.5 | 1.5 | 3.0 (2016) | yes |
| CB | Samuel Umtiti (Lyon) | 23 | 71 | 15.0 | 70.0 | 45.0 | 70.0 (2018) | yes |
| CB | Marquinhos (PSG) | 22 | 66 | 30.0 | 55.0 | 65.0 | 75.0 (2021) | yes |
| CB | John Stones (Everton) | 22 | 61 | 28.0 | 55.0 | 60.0 | 60.0 (2018) | yes |
| ST | Michy Batshuayi (Marseille) | 23 | 71 | 15.0 | 40.0 | 30.0 | 40.0 (2018) | yes |
| ST | Aleksandar Mitrović (Newcastle) | 22 | 62 | 14.0 | 15.0 | 25.0 | 28.0 (2022) | yes |
| ST | Paulo Dybala (Juventus) | 23 | 60 | 40.0 | 110.0 | 85.0 | 110.0 (2018) | yes |

### 3. Selected players versus the other young regular starters (79 players)

| | Selected (22) | Others (79) |
|---|---|---|
| Median starting value (2016) | €10.0M | €7.0M |
| Median value in 2019 | €35.0M | €20.0M |
| Peak value of €20M or more | 82% | 57% (Fisher p = 0.046) |
| Peak value of €50M or more | 36% | 24% |
| 900+ minutes in the top-5 leagues in 2018/19 or 2019/20 | 82% | 82% (p = 1.0) |
| Median growth in value to 2019 | +119% | +206% |

The selected players started more expensive, so the higher peaks are partly a starting-price effect. Regression of growth
to 2019 on selection, starting value, age and position group: **+10% (95% CI −27% to +67%, p = 0.65)**. The groups are small,
so this means "no evidence of an advantage", not "no advantage".

### 4. Goalkeepers

Goalkeeper metrics are weaker: open data have no post-shot xG, so shot-stopping is measured by save percentage on shots on target
(non-penalty), non-penalty xG against minus goals conceded, plus passing, long passes, sweeping and claiming. The best
young goalkeepers by this score (value in EUR millions):

| Rank | Goalkeeper (2015/16 team) | Age | 2016 | 2018 | 2019 | 2021 | Peak (year) | Top-5 league minutes 2018/19 | 2019/20 |
|---|---|---|---|---|---|---|---|---|---|
| 1 | Yoan Cardinale (Nice) | 22 | 0.6 | 3.0 | 2.0 | 0.6 | 5.5 (2017) | 270 | 0 |
| 2 | Sergio Rico (Sevilla) | 23 | 15.0 | 12.0 | 12.0 | 7.0 | 20.0 (2017) | 2,610 | 180 |
| 3 | Gianluigi Donnarumma (Milan) | 17 | 8.0 | 40.0 | 55.0 | 65.0 | 65.0 (2021) | 3,092 | 2,302 |
| 4 | Pierluigi Gollini (Verona) | 21 | 2.0 | 3.5 | 6.0 | 17.0 | 17.0 (2020) | 1,800 | 2,250 |
| 5 | Paul Bernardoni (Bordeaux) | 19 | 1.2 | 2.0 | 9.0 | 10.0 | 10.0 (2021) | 3,420 | 2,204 |
| 6 | Pau López (Espanyol) | 22 | 1.5 | 5.0 | 20.0 | 10.0 | 24.0 (2019) | 2,970 | 2,250 |
| 7 | Alban Lafont (Toulouse) | 17 | 0.8 | 18.0 | 17.0 | 10.0 | 20.0 (2023) | 3,015 | 2,430 |

Of the three selected, one became a star, two did not. All four who were ranked lower settled in the top leagues. With seven
goalkeepers this is an illustration, not a result.

## What this shows

- Position-specific statistics do pick out good young players: most of the selected 22 became regulars in the top leagues and
  several became very valuable.
- But the selection was **not clearly better than simply taking other young regular starters**. Once starting price and age
  are accounted for, I find no advantage, and the share who stayed in the top leagues was identical (82%).
- Three of the clearest misses (Cabot, Sylla, Juncà) played for small clubs. A possible reason is that defensive numbers are
  inflated for players on teams that spend more time without the ball. The possession adjustment removes only part of this.
  I did not test it.
- A season of statistics measures how well a player performed in a given team. It does not measure how much he will
  improve, which matters most for under-23s.

## Limitations

- **One season, four leagues, 22 selected players.** Differences between groups are small relative to the noise. Many metrics
  and several comparisons were run; only the pre-defined comparison above is reported as the main result.
- **Choices made by me:** the metric sets (taken from published material but still my selection), shrinkage, possession
  adjustment, cut-offs and the extension of the fallback rule described above.
- **Event data only:** no off-ball movement, pressing structure, physical data or video. Defensive metrics are noisier and
  more dependent on team style than attacking ones.
- **Age:** 19 players had no birth date in Transfermarkt and could not be assessed. Percentiles use players of all ages
  (900+ minutes).
- **Transfermarkt values** are crowd-sourced and updated a few times a year; a "June" value may date from earlier.
  The peak value is the maximum recorded up to June 2026, so players who were still developing may peak later.
  Careers are shaped by injuries, club fit and luck as well as ability.
- **Goalkeepers:** no post-shot xG, and xG against minus goals also depends on the defence in front of the goalkeeper.
  Seven players is too few for conclusions.
- Roles come from the most frequent position label. A few details of the open data: three Ligue 1 matches are missing, and one
  club appears under two names.

## Earlier analyses (notebooks)

Before this design I ran an exploration that used market values directly:
- The market paid for goal threat, attacking output and ball progression, and almost nothing for defensive qualities.
- On leagues the model had not seen, adding performance profiles to age and starting value did **not** significantly improve
  predictions of value growth (gain of 1–2 percentage points, intervals include zero).
- An early back-test looked strong (+20% / +33% / +49%) on the leagues used for tuning but shrank to +6% / +16% / +13%
  (not significant) on unseen leagues. I treat the second set as the result.

The notebooks are in [`notebooks/`](notebooks/): the exploration and source linking, and the under-23 scouting study.

## Data attribution

Event data provided by StatsBomb: https://github.com/statsbomb/open-data

![StatsBomb logo](../hudl-statsbomb-logo-default.png)

Market values and appearances from the open Transfermarkt dataset (CC0):
https://github.com/dcaribou/transfermarkt-datasets
