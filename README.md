# MultiplePlatformBayesianNetworks
Associated files for Shaddox E, Peterson CB, Stingo FC, Hanania N, Cruickshank-Quinn C, Kechris K, Bowler R, Vannucci M. (2020) Bayesian inference of networks across multiple sample groups and data types. *Biostatistics*. 21(3): 561–576.

Author: Elin Shaddox


The provided Matlab, R, and supplementary files for Bayesian inference of multiple graphical models across multiple platforms are associated with the following publication:
- Shaddox E, Peterson CB, Stingo FC, Hanania N, Cruickshank-Quinn C, Kechris K, Bowler R, Vannucci M. (2020) Bayesian inference of networks across multiple sample groups and data types. *Biostatistics*. 21(3): 561–576.

These scripts rely on functions from the Matlab code originallly provided by Hao Wang associated with the following publication:
- Wang H, Scaling it up: Stochastic search structure learning in graphical models. *Bayesian Analysis*. 10(2015): 351-377

In addition, the code relies on aspects of the implementation for the following publiction:
- Shaddox E, Stingo F, Peterson CB, Jacobson S, Cruickshank-Quinn C, Kechris K, Bowler R, Vannucci, M. (2018). A Bayesian approach for learning gene networks underlying disease severity in COPD. *Statistics in Biosciences*. 10(1): 59–85.

Please cite all publications if you use this code. Thanks!

### OVERVIEW OF FILES 


### Example_multiple_graphs_SSVS_with_platforms.m

Basic example of running the MCMC sampler and generating results summaries on a simple setting with:
- Platform 1 - 3 groups with identical dependence structure
- Platform 2 - 3 groups with differing dependence structure

### MCMC_multiple_graphs_SSVS_with_platforms.m
Code for running the MCMC sampler

### calc_mrf_C.m
Helper function for calculating the normalizing constant for the MRF prior

### Data generation for simulations
Scripts to generate matrices similar to those from simulation settings:
- ScaleFreeSimTruths_p40.R: input (true precision matrices) for generating data for p=40 simulations in ScaleFreeSimDataGeneration.m
- count_shared_edges.m: a matlab function for counting edges between two adjacency matrix inputs
- AR2_SimulationTruthsAndDataGeneration.m: set up for true precision matrices and data generation in AR(2) p=80 simulation settings


### Metabolite selection example
Script, plots, and generated data to provide an example of correlated metabolite data and the iterative metabolite selection process from the publication listed above:
- MetaboliteExampleSelection.R: script for data generation and iterative process
- corData_MetabSelectionExample.csv: generated data based on correlation of a metabolite subset
- BEFORESELECTIONgeneratedCorrDataPlots.png: plot of correlated data before selection
- AFTERSELECTIONgeneratedCorrDataPlots.png: plot of less correlated data subset after selection
