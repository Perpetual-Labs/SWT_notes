Infer results from data given, if the data is provided in a [[Semantics|semantic]] way

Reasoners act as a compiler - compile the model to generate results

In particular, practical reasoning algorithms exist that are both:		
	sound: all inferences drawn are valid	
	complete: all valid inferences are drawn	

These algorithms have been implemented in both commercial and free software that is widely used.

In addition, these reasoners can detect various errors such as inconsistencies or unsatisfiable (i.e., overconstrained) classes.

Information expressed in [[OWL]] can be semantically validated, we have an opportunity to catch errors on every exchange.

Reasoners provide the ability to ask questions about information, e.g.
- What is the measured mass of the flight system?
- What are all the (recursively) contained components of the flight system?
- What requirements refine R.12345?
- Does every component have a supplier?

## Languages:
[[OWL]] already has a lot of reasoning power
[[SWRL]] can generate more data
SHAQL mostly used for checking constraints
You can combine them


References
[[Jenkins - ST4SE]]