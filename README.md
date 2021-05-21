# 18335 Final Paper
This folder contains several Julia scripts. 

VEGAS.jl is our implementation of the VEGAS algorithm. It takes as input the function to be integrated f, D the number of dimensions, bounds a [2, D] matrix with lower bound on the first row and upper bound on the second row, and max_evals which is the maximum number of iterations. Hyperparameters such as iter_max or the number of iterations, N the number of samples per iteration, M the number of intervals, and alpha the damping constant. Returned is the integral estimate and standard deviation. 

We also provide our code for the brute force Monte Carlo in Monte_Carlo.jl with the same input and output as VEGAS.jl.

Finally, testing.jl reproduces plots included in the paper with several other examples available. Note that the Cuba library algorithms all require bounds to be [0, 1], so we must provide a different function for these with the transformation to this region. 
