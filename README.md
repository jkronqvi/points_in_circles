# points_in_circles
This repository contains a collection of MINLP test instances available in both .nl and .gms format.

The underlying optimization task is simple, select n-points in m-dimensional balls, such that the l1-distance between all points is minimized. Only one point can be assigned to each ball, and in total there are l-balls with radius one. 

There are two versions of each problem, one with the Big-M formulation and one wtith the convex hull formulation presented in [1]. The convex hull models all have the _H extension to the file name. All models have been generated with Pyomo modelling framework [2,3].

These test problems are designed to be challenging both due to the nonlinearity and the combinatorial aspects. It is well known that it is challenging to create and accurate polyhedral outer approximation of an m-dimensional ball without any reformulations [4, 5], and this renders the problems challenging for polyhedral outer approximation based solvers.

The names of the problems also describe the main properties, e.g, the instance p_ball_30b_10p_2d_H contains 30 2-dimentional balls, 10 points and uses the convex hull formulation.

The file "generate_test_problems" contains a simple puthon script for generating test problems of different size with both the big-M and convex hull formulation using Pyomo.

References:

[1] Sawaya NW, Grossmann IE (2007) Computational implementation of nonlinear convex hull reformulation. Computers & Chemical Engineering

[2] Hart WE, Laird CD, Watson J-P, Woodruff DL, Hackebeil GA, Nicholson BL, Siirola JD (2017) Pyomo – Optimization Modeling in Python. Second Edition.  Vol. 67. Springer.

[3] Hart WE, Watson J-P, Woodruff DL (2011) Pyomo: modeling and solving mathematical programs in Python. Mathematical Programming Computation.

[4] Hijazi H, Bonami P, Ouorou A (2013) An outer-inner approximation for separable mixed-integer nonlinear programs. INFORMS Journal on Computing.

[5] Kronqvist J, Lundell A, Westerlund T (2018) Reformulations for utilizing separability when solving convex MINLP problems. Journal of Global Optimization.
