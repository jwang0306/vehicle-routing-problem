# Vehicle Routing Problem - Traveling around Europe

This is a project that demonstrates vechicle routing problem. We solved it with Linear Programming using pulp package, which yields the optimal solution.

## Dataset

The data is collected by web crawling from the [traveling site](), which can be found in ```data``` folder as csv file. Here are the informaions:

- 24 capitals
- distance
- flight time
- longitude  & latitude

## Prerequisites

- python
- pulp
- matplotlib
- seaborn
- numpy
- pandas

## Usage

Run ```vrp.ipynb``` to plot the result. You can set varaible K to indicate numbers of salesmen. Note that K greater than 4 might take hours.

## Result Diagrams

- 1 person (Wall time: 1min 3s)
    - Longest time spent: 6494 (min)
    - Total distance: 12287.07 (km)

    ![](https://i.imgur.com/khy8Lek.png)

- 2 people (Wall time: 4.66 s)
    - Longest time spent: 3574 (min)
    - Total distance: 12607.64 (km)

    ![](https://i.imgur.com/5NM2ZQ1.png)

- 3 people (Wall time: 14min 48s)
    - Longest time spent: 2546 (min)
    - Total distance: 14130.25 (km)

    ![](https://i.imgur.com/mFugpKP.png)

- 4 people (Wall time: 44min 58s)
    - Longest time spent: 1988 (min)
    - Total distance: 15425.02 (km)

    ![](https://i.imgur.com/EIDcAlH.png)

Once **K (num of salesmen)** is larger, it is better not to solve it with linear programming. We should use meta heuristic methods instead, though the solution might not be optimal, yet a lot faster.


## A star would be nice if you like it !
