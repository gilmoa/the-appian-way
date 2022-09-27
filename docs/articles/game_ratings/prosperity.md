---
sidebar_position: 1
description: "Arguably the most challenging rating in the game, Prosperity causes problems to the newcomer and seasoned pro alike. Whether you want tips on how to squeeze those last few prosperity points out of a map, or an in-depth discussion of the finer points of Prosperity calculations - here is the place to be!"
---

# Prosperity Rating

Of all the ratings in the game, Prosperity is most often the scourge of Governors. It is almost invariably the first significant hurdle that faces most new governors, and can drive even the most experienced of us to the brink of insanity. If you've reached the point where your hair is now kept in a paper bag, then I'm probably a bit late... but you might like to read on anyway.

## The Prosperity Cap

The manual lists a large number of factors that contribute to the prosperity rating. What it fails to mention is that the prosperity rating is capped. However many of the criteria you fulfil, once you reach the 'prosperity cap, it will rise no further.

How then, is this mysterious 'prosperity cap' determined? It is helpful to know that each housing level has a characteristic prosperity factor (found in the depths of C3_Model.txt), which are summarised in the table below. The prosperity cap is given by the mean value of this prosperity factor.

| Housing Level      | Prosperity Cap | Housing Level     | Prosperity Cap |
| ------------------ | :------------: | ----------------- | :------------: |
| **Small Tent**     |       5        | **Large Insulae** |       65       |
| **Large Tent**     |       10       | **Grand Insulae** |       80       |
| **Small Shack**    |       15       | **Small Villa**   |      150       |
| **Large Shack**    |       20       | **Medium Villa**  |      180       |
| **Small Hovel**    |       25       | **Large Villa**   |      400       |
| **Large Hovel**    |       30       | **Grand Villa**   |      600       |
| **Small Casa**     |       35       | **Small Palace**  |      700       |
| **Large Casa**     |       45       | **Medium Palace** |      900       |
| **Small Insulae**  |       50       | **Large Palace**  |      1500      |
| **Medium Insulae** |       58       | **Luxury Palace** |      1750      |

The prosperity cap for the city is simply the average value of the prosperity factor calculated over all the houses in the city.

```math title="Prosperity Rating Formula"
Prosperity Cap = AVG([N_HousingLevel * ProsperityHousing])

Prosperity Cap = [(N small tents * 5) + (N large tents * 10) + ... + (N luxury palaces * 1750)] / N houses
```

To make life easier, here's an example. For a city with 5 large tents, 200 small casa, and 4 luxury palaces we obtain:

```math title="Prosperity Rating Example"
Prosperity Cap = [(5 * 10) + (200 * 35) + (4 * 1750)] / 209 = 67
```

So the highest possible Prosperity rating in such a hypothetical city would be 67.

As can clearly be seen, the Prosperity factors are heavily weighted towards the higher echelons of housing. Villas, and palaces in particular, have ludicrously high prosperity factors. They also pay an awful lot in taxes. Thus, it is far easier to attain a mid-range or high prosperity target (say 45 or over) with a small number of highly evolved houses, and a lot of lower-level houses, than it is to evolve all houses to a uniform intermediate stage. The problem, of course, then becomes one of building stable high-level housing. See the 'housing blocks' section for more details on how to get those patricians to move in (and stay in residence).

A further point of interest arises for houses below large insulae, which can exist in both 1x1 and 2x2 forms. A single 2x2 and a single 1x1 both count as one house. More to the point, four 1x1 houses occupying the space that might be filled by a 2x2 count as four houses. If the houses in question are relatively low-status, then the four 1x1's will dent your prosperity rating more than the single 2x2. The problem of 1x1 versus 2x2 is discussed in full elsewhere.

## Prosperity Increases

The second problem with prosperity rating is that it is only calculated once a year, and it can rise very slowly. If you have improved your prosperity cap by 40 points in a year, which is not inconceivable, you will not receive a 40 point boost to your prosperity in January. If your prosperity cap is higher than your current prosperity rating, prosperity will rise 2 points, with additional bonuses or penalties as follows:

- +2 Your city makes a profit[^1]
- +1 10% or more of your population lives in villas
- +1 Less than 30% of your population lives in tents or shacks
- +1 Active Hippodrome
- +1 Less than 5% unemployment
- +1 There is at least one Grand Insula or better in your city
- +1 You pay at least 2 Dn more than Rome's wage
- -1 City loses money[^1]
- -1 Unemployment rate is above 15%
- -1 Your wages are below Rome's
- -3 You go broke and Caesar bails you out
- -3 Failure to pay tribute

[^1]: Your city is deemed to make a profit provided you lose less money than you spend on construction.

As you can see, improving your housing alone is not sufficient to ensure a rise in prosperity. All told, an 8-point prosperity rise in one year is extremely good, and if you manage the full ten, then you are a probably a C3 deity. The importance of having sufficient money in the treasury at year end to pay tribute cannot be overemphasised. Failure to pay tribute doesn't just hammer your prosperity rating, but it will also do untold damage to your favour rating.

All the game data used was originally presented by Donald Irvine, on his excellent website Which Way to Rome?
