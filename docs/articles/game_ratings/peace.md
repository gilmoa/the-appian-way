---
sidebar_position: 4
description: "A brief discourse on the finer points of peace rating calculations."
---
# Peace Rating

My fourth and final article on the in-game ratings concerns the peace rating. Although most of the information contained herein is fairly old stuff, there is one new piece of information: the effect of protestors on the peace rating. The relationship outlined below was first suggested by wolf, a frequent contributor to all the Caesar 3 forums. Subsequent tests by myself have verified his original theory.

In many respects, peace is the simplest of the in-game ratings: it rises steadily with time, unless buildings in the city are damaged by invasions or riots. For those of you who prefer cold, hard numbers to general descriptions, a more detailed discussion now follows.

## The Numbers

For the first two years of a scenario, peace rises by two points per year. Thereafter, your citizens feel more secure, and the peace rating rises by five points per year.

These basic rises are then subject to the following modifiers:

- -1 If any house in the city spawns a protestor during the year (there are no further penalties for the second and subsequent protesters spawned).
- -1 For each of the first twelve buildings destroyed by invaders or rioters

Certain buildings are classified as defensive (or defensive support) structures, and may be lost without penalty. These are:

- Walls
- Gatehouses
- Towers
- Prefectures
- Aqueducts
- Engineers' Posts
- Tents
- Wells

Invasion and riot damage carries a further penalty. For two years following damage by riots or an invasion, the peace rating rises by at most two points (just like in the first two years of the scenario). presumably this is intended to reflect your citizens' renewed concerns for their safety.

## Worked Examples

Consider a city where an invasion in year 4 destroys one building, and a second invasion in year 8 destroys eight buildings. The peace rating would change with time as follows:

|      Date       | Peace Rating |       Date       | Peace Rating |
| :-------------: | :----------: | :--------------: | :----------: |
| January, Year 1 |      2       | January, Year 7  |      22      |
| January, Year 2 |      4       | January, Year 8  |      27      |
| January, Year 3 |      9       | January, Year 9  |      24      |
| January, Year 4 |      14      | January, Year 10 |      26      |
| January, Year 5 |      18      | January, Year 11 |      28      |
| January, Year 6 |      20      | January, Year 12 |      33      |

Now consider a city in which a criminal is spawned in years 1 and 4. The Peace rating would change as follows:

|      Date       | Peace Rating |      Date       | Peace Rating |
| :-------------: | :----------: | :-------------: | :----------: |
| January, Year 1 |      2       | January, Year 4 |      13      |
| January, Year 2 |      3       | January, Year 5 |      17      |
| January, Year 3 |      8       | January, Year 6 |      22      |
