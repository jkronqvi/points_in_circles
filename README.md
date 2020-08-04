# points_in_circles
This repository contains a collection of MINLP test instances available in both .nl and .gms format.

The underlying optimization task is simple, select n-points in m-dimensional balls, such that the l1-distance between all points is minimized. Only one point can be assigned to each ball, and in total there are l-balls with radius one. 

There are two versions of each problem, one with the Big-M formulation and one wtith the convex hull formulation presented in [1]. The convex hull models all have the _H extension to the file name. 

References:
[1] Sawaya  NW,  Grossmann  IE  (2007)  Computational  implementation  of  non-linear  convex  hull  reformulation.  Computers  &  Chemical  Engineering
