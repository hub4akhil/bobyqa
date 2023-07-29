# bobyqa

The code generates an ini for bobyqa algorithm in cosmomc.

By default it keep the following setting:

 - minimize_random_start_pos = F
 - use_fast_slow = T
 - max_like_radius = 0.005
 - max_like_iterations = 5000
 - minimization_points_factor = 4
 - minimize_loglike_tolerance = 0.05
 - minimize_separate_fast = F \
   
   To do some low temperature MCMC steps to check minimum stable
 - minimize_mcmc_refine_num = 50
 - minimize_refine_temp = 0.01 
\

The code also changes the ranges starting values reading the corresponding likestat values they obtained from MCMC run.

## How to run the code?
 The code takes two inputs : 
1. Likestat file of mcmc run
2. ini file corresponding to the MCMC run

Make sure that MCMC ini file is also present in the bobyqa code base.

Using the syntax to run the code
```
py bbqa_ini.py <likestat file> <mcmc ini>
```
