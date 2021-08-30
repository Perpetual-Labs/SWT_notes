## Design for Additive Manufacturing (DFAM) [[Ontology]]

#### Overview

[[Ontology]] for [[Additive Manufacturing]]
Built in [[OWL]] and [[Protege]]
Queries using [[SWRL]]


#### Interesting Terms

 - Design feature
	 - geometric regions of a part model that represent design intent and support reasoning.
 - Geometry parameter
	 - comprisedBy Design features
	 - similar to PhysicalQuality
 - Manufacturing feature
	 - evaluates a Geometry parameter - to do with manufacturing process.
	 - Used to indicate and classify design features that may violate manufacturing constraints
 - Material parameter
	 - e.g. material type
 - Process parameter
	 - similar to FunctionalQuality
	 - e.g. laser power

![[DFAM Ontology.jpg]]


#### Issues

There is no representation aspect
i.e. no use of something like the [[IAO]]
The design and manufacturing features are simialrly captured in [[FPRO]]


#### References
[[Kim2019 - A design for additive manufacturing ontology to support manufacturability analysis]]
[[Kim2018 - Linking part design to process planning by design for additive manufacturing ontology]]