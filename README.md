# bargaining-equilibrium-exist
Replication code for the simulations in the lates version of "Nash-in-Nash Equilibrium with Inefficient Prices". 

Please email me at dc5004@nyu.edu if you find typos or mistakes.

These simulations are for the multiproduct mixed-logit oligopoly in Section 7. 

Each notebook is self-contained, and has the code for the differenti robusness checks mentioned in Appendix D.

The main computational cost comes from the grid size. With 35 grid points in each dimension of X, the code
runs in 60-70 minutes in a MacBook Air with an M2 chip and 8gb of RAM. 

The largest grid has 54 grid points in each dimension (for a total of over 8,503,056 grid points)
and runs in aroud 6 hours, depending on machine conditions.

Each notebook runs the following code.

1. notebook_1_main.ipynb outputs figure 1 of the paper.
2. notebook_2_gamma.ipynb sets gamma = 1 instead of = 0. Gamma is a parameter in the marginal cost function.
3. notebook_3_lognormal.ipynb uses a lognormal distribution for alpha.
4. notebook_4_larger_alpha.ipynb uses a lognormal distribution for alpha, with a higher mean.
5. notebook_5_full_heterogeneity.ipynb has heterogeneity in both price and product characteristic parameters.
6. notebook_6_bargaining_seed.ipynb uses a different seed to generate the bargaining parameters.
7. notebook_7_pyblp_seed.ipynb uses a different pyblp seed.
