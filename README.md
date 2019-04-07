# Python Ant Colony TSP Solver

Uses Ant Colony Optimization to solve the TSP.  
See http://en.wikipedia.org/wiki/Ant_colony_optimization_algorithms 

**anttsp.py** is the file to run.  It reads from citiesAndDistances.pickled, which is a pickled 2D array with this format:

| CityName1 | CityName2 | ... | CitNameN |
|-----------|-----------|-----|----------|
| 0         | 23        | ... | 34       |
| 10        | 0         | ... | 22       |
| .         | .         | .   | .        |
| .         | .         | .   | .        |

It is not necessary for the matrix to be symmetric i.e. the distance traveling from A to B need not be the distance from B to A  (if you have ever been to Italy and dealt with the mess of one-way streets you will understand how this applies).

Run without additional arguments, it solves the 10-city TSP

You can also try this:
```
$ python anttsp.py 14
```

Other values <= 14 tested as well

