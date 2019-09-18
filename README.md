# Vehicle Routing Problem - Traveling around Europe

This is a project that implements a simple real-life demo of Vehicle Routing Problem (VRP). The question definition is to conqure Travel Salesman Probelm (TSP) that has multiple salesm"e"n.

## Motivation

This is a project of the course Operating Research. My friend and I are imaging that, one day we'll travel the entire Europe together. We initially form this as a TSP problem, but soon we realize that it would be better if we all take different route and share our experiences afterwards. Therefore it became a VRP.

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

Once **K (num of salesmen)** is larger, it is better not to solve it as a linear problem using pulp package. We should use meta heuristic methods instead, though the solution might not be optimal, yet a lot faster.

## STAR THIS REPO if you like it !
