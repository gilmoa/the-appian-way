---
sidebar_position: 3
description: "Yields from farming and fishing, and the appetite of the Roman citizen are all quantified and discussed here."
---
# Feeding Folks

One of the earliest pieces of game data elucidated about C3 were the production rates of farms, raw material producers, and workshops. However, until extremely recently, fishing has remained a comparatively poorly understood part of C3. Now, thanks to the work of my fellow governor, Dorito the Merciless, it is a mystery no more.

Anyway, enough rambling. It's to time to get back to cold, hard, game data. Before I look at the various food sources in turn, I shall examine the appetite of the C3 citizen.

## Food Consumption

Citizens in C3 consume food at the rate of 6 units per year. The use of the term 'unit' can cause a little confusion, so I'll try and give a decent explanation. When food is stored in a granary, it is measured in 'cartloads'. When food is transferred from granary to market, one cartload is broken down into 100 units. So, one cartload of produce is 100 units, enough to feed 16.66 people for a year.

When housing reaches Grand Insulae, it begins to consume a second food type, and a third is consumed at Grand Villa or above. When a house uses multiple food types, food consumption is divided equally between them i.e. occupants of Grand Insulae consume three units per year of the two food types, and occupants of Grand Villas consume 2 units per year of the three types.

With this information under our belt, it is time to look at the productivity (in cartloads per year) of the two food sources in C3: farming and fishing.

## Farming

Farms are almost tediously predictable. With one important exception, farms produce 9.6 cartloads of food per year. The one exception is Wheat farms in Central and Desert provinces; these are twice as productive as other farms, and produce 19.2 cartloads per year.

However, the productivity of a farm is critically dependent on the proximity of a granary accepting the relevant food type. A farm has only one cartpusher. If that cartpusher has not returned from his last delivery when a farm reaches 100% productivity, then the farm will stand idle until he returns. In order to maintain maximum productivity from a Central/Desert wheat farm, there must be a granary accepting wheat within 16 tiles of the farm. All other farms require an accepting granary within 32 tiles.

In case you were wondering, these numbers are derived on the basis that a central/desert wheat farm cartpusher needs to make 19.2 return trips to a granary in the year. If we divide the walker speed (640 tiles/year) by 38.4 distances/year, we obtain the maximum granary distance of 16 tiles. For other farms, we simply double this number.

Consequently, we arrive at the following table, which gives the maximum number of people the two types of farm can feed:

| Food Source | People Fed |
| :---------- | :--------: |
| Wheat Farm  |    320     |
| Other Farm  |    160     |

## Fishing

Fishing is a little more complicated. Once you have manned your fishing wharf, and supplied it with a fishing boat from a shipyard, then the fisherman have several tasks to fulfil:

- Sail to the fishing grounds
- Catch the fish
- Sail back to the wharf
- Unload the catch

Each of these steps takes time: the sailing to and from the fishing grounds takes place at the standard rate of 640 tiles/year. Catching the fish uses up 14 tiles worth of time, and unloading uses a further 3 tiles worth. Hence, we obtain the fishing productivity formula:

```math title="Fishing Productivity Formula"
640 / (17 + 2 * (distance to wharf in tiles)) Cartloads/Year
```

In order to maintain maximum productivity, a granary accepting fish must be located no more than five tiles further from the wharf than the fishing spot. We now apply the magic formula, to obtain the maximum number of people a wharf can feed at various distances from a fishing spot.

| Distance from fishing spot (in tiles) | Annual Production (cartloads) | People fed |
| :-----------------------------------: | :---------------------------: | :--------: |
|                   0                   |             37.6              |    627     |
|                   1                   |             33.7              |    561     |
|                   2                   |             30.5              |    507     |
|                   3                   |             27.8              |    463     |
|                   4                   |             25.6              |    426     |
|                   5                   |             23.7              |    395     |
|                   7                   |             20.6              |    343     |
|                  10                   |             17.3              |    288     |
|                  15                   |             13.6              |    226     |
|                  20                   |             11.2              |    187     |

As can be seen, when wharves are close to fishing grounds, yields of fish are spectacularly high. When you take into account the fact that wharves have fewer employees than farms, there can be little doubt that fishing is almost always the most labour-efficient way of feeding your population. So remember to treat your fisherman well!
