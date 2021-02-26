## Types of Simulation:
Causal 
 - This is a limitation of the Biomass and ExoMars models
 - input/output simulation - chain of simulation tools
 - this approach breaks down with co-deoendent blocks and feedback loops
 - need 'continuous integration'
Acausal
 - more powerful and intuitive
 - [[Modelica]] and [[Simscape]] implement this
 - e.g. [[Simulink]] is causal, [[Simscape]] is acausal
 - requires Functional Mock-up Interface (FMI)
 - Can run on High-Performance Computing (HPC) cloud
 - can develop simulation blocks in parallel
 - Linked to [[Knowledge Graph]] (continuous integration)
 - BUT: very computationally expensive, especially physics models (e.g. CFD)
 - SOLUTION: [[Surrogate Modelling]]
 - This requires machine-learning (i.e. what [[Hartree Centre]] are developing)


References:
[[Gregory2019 - Investigating the Flexibility of the MBSE Approach to the Biomass Mission]]