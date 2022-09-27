---
sidebar_position: 2
description: "Whether you want to know how the Culture Rating is calculated, or simply how best to bolster your rating, here is the place to look."
---
# Culture Vulture

After the Prosperity rating, the Culture rating is usually the second biggest problem faced by a governor in a city. Being an extremely dull man, I have often wondered exactly how the Culture rating is calculated. Now, thanks to some excellent work by catilina, a regular contributor to the forums at C3 Heaven you and I can now both find out...

## Which buildings will improve my culture rating?

The only buildings that contribute to the Culture rating are:

- **Religious buildings**:
Small Temples, Large Temples, and Oracles
- **Education Buildings**:
Schools, Academies and Libraries
- **Entertainment Venues**:
Actually, only Theatres contribute. All the remaining entertainment venues do not contribute to the Culture rating at all.

## OK, so how does it work?

Much like the system for awarding bonus entertainment points for citywide coverage (see this page for more details), the Culture rating is based on coverage indices for the various buildings. A coverage index for a particular building is calculated as follows:

```math title="Culture Rating Formula"
[(number of buildings) * (building coverage)] / (city population)
```

Note that for Schools and Academies the city population is not used. For Schools the number of schoolchildren in the city is used, and for Academies the number of young people is used. Both of these figures vary according to city demographics, and can be found by consulting your population advisor.

The building coverage is the number of people served by each building. The following table summarises this for all the relevant buildings:

| **Building**                | Building Coverage |
| --------------------------- | ----------------- |
| **Small Temple (Set of 5)** | 750 People        |
| **Large Temple (set of 5)** | 1500 People       |
| **Oracle**                  | 500 People        |
| **School**                  | 75 Schoolchildren |
| **Academy**                 | 100 Young People  |
| **Library**                 | 800 People        |
| **Theatre**                 | 500 People        |

Once you have calculated the coverage indices for the various buildings, the coverage indices for the three types of religious buildings are then summed to give an overall religion coverage index. Culture thus depends on five coverage indices:

- Religion
- Theatres
- Libraries
- Schools
- Academies

Culture points are awarded based on these coverage indices, using a non-linear scaling detailed in the following table:

| **Coverage Index** | 1 or more | 0.99-0.86 | 0.85-0.71 | 0.70-0.51 | 0.50-0.31 | 0.30-0.00 |
| ------------------ | :-------: | :-------: | :-------: | :-------: | :-------: | :-------: |
| **Religion**       |    30     |    22     |    14     |     9     |     3     |     0     |
| **Theatres**       |    25     |    18     |    12     |     8     |     3     |     0     |
| **Libraries**      |    20     |    14     |     8     |     4     |     2     |     0     |
| **Schools**        |    15     |    10     |     6     |     4     |     1     |     0     |
| **Academies**      |    10     |     7     |     4     |     2     |     1     |     0     |

As you can see, there is a great deal to be gained by improving the coverage of a building from almost perfect to perfect (more so than improving from none to a small amount). Further, the culture rating is heavily biased towards religion, Theatres and Libraries, with comparatively few points available for Schools and Academies.

One further word of caution: for cities with populations below about 300, all the Culture calculations (and a number of other things) go out the window. Quite simply, these calculations will not work for a city of such a small size.

## A Sample Calculation

We take as an example a city of 10254 people, with 526 Schoolchildren, and 247 young people. This city has 3 sets of 5 Small Temples, 12 Oracles, 10 Theatres, 8 Schools, 2 Academies, and 8 Libraries.

```math title="Calculate coverage indices"
Religion:  [(12 * 500) + (3 * 750)] / 10254 = 0.80
Theaters:  (10 * 500)               / 10254 = 0.49
Schools:   (8 * 75)                 /   526 = 1.14
Academies: (2 * 100)                /   247 = 0.81
Libraries: (8 * 800)                / 10524 = 0.61
```

```math title="Culture points"
Religion: 14
Theaters:  3
Schools:  15
Academies: 4
Libraries: 4
------------
Total:    40
```

## More on coverage indices

Your advisors will report overall citywide coverage for Culture venues, and the mood of the goods, based on coverage indices. The following table summarises this for citywide coverage of Schools, Libraries, Academies, and Theaters. This also applies to other entertainment venues and to Hospitals.

| **Coverage Index** | Advisor reports | **Coverage Index** | Advisor reports |
| :----------------: | --------------- | :----------------: | --------------- |
|      **1.00**      | Perfect         |   **0.40-0.59**    | Average         |
|   **0.90-0.99**    | Excellent       |   **0.30-0.39**    | Below Average   |
|   **0.80-0.89**    | Very Good       |   **0.20-0.29**    | Poor            |
|   **0.70-0.79**    | Good            |   **0.10-0.19**    | Very Poor       |
|   **0.60-0.69**    | Above Average   |   **0.00-0.09**    | None            |

The mood of the gods, as reported by your religious advisor, depends on the religion coverage index:

| **Coverage Index** | God's mood  | **Coverage Index** | God's mood |
| :----------------: | ----------- | :----------------: | ---------- |
|   **0.98-1.00**    | Happy       |   **0.58-0.67**    | Irritated  |
|   **0.88-0.97**    | Pleased     |   **0.48-0.57**    | Angry      |
|   **0.78-0.87**    | Indifferent |   **0.38-0.47**    | Very Angry |
|   **0.68-0.77**    | Displeased  |   **0.00-0.37**    | Wrathful   |

Should you choose to ignore any of the gods, then naturally their mood will worsen. The same coverage index calculation can then be made to determine the mood of that god. I would not, however, advise you to irritate the gods: their wrath, though rarely catastrophic, is often a major nuisance.
