## PSO: Physics-based Simulation [[Ontology]]

#### Overview

Built on [[BFO]] and [[IAO]]
Developed by [[Hyunmin Cheong]]


#### Modules

PSO-Physics:
 - terms and relations used to model physical phenomena based on the persepctive of classical mechanics involving PDEs
 - used to model the physical phenomena of interest independent of solver-specific operations, which can be reused across different solvers

PSO-Sim:
 - terms used to represent the information artifacts that are about the physical phenomena modelled with PSO-Physics
 - used to instantiate solver-specific input-data

This distinction between the physical world and the information used to describe it is key

#### Assumptions

- Classical mechanics
- Ignore quantum mechanics, quantum field theory, relatavistic effects
- Does not need to solve behaviour (this is for specific solvers), just capture sufficient snapshots to initiate solvers


#### Useful Terms

 - Physical Property
 - Material Property

Also interesting to note that the solution to designing a system is:
 - system does not exist yet
 - but it is possible in the laws of physics
 - so it is treated as if it is a real object (ie independent continuant)


#### References:
[[Cheong2019 - Physics-based simulation ontology. an ontology tosupport modelling and reuse of data for physics-based simulation]]