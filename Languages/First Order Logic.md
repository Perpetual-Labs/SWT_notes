## Overview
In First Order Logic (FOL), there are Quantors which allow assertions about sets of objects, without naming the objects explicitly. Example:
	- All humans are mortal
	- Socrates is a human
	- Induction: Socrates is mortal

## Model-theoretic [[Semantics]]
 - Interpretation - assignment of meaning to the symbols of a formal language
 - Interpretation is given by in 'model-theoretic semantics' by mapping the terms (TBox) to the individuals (ABox)
 - i.e. from propositions to truth values


## Variants of FOL rules:
Clause: 
- more than one atomic type in header (disjunctive example)
- Person(x) -> Woman(x) ∨ Man(x)
Definite clause:
- only onw atomic type in header
- Man(x) ∧ hasChild(x,y) -> Father(x)
Functional clause:
- function in premise
- hasBrother(mother(x), y) -> isUncleOf(y,x)
Horn clause:
 - conjunctive elements in the premise
 - the example below implies nothing i.e. impossible
 - Man(x) ∧ Woman(x) ->
Fact:
 - e.g. Woman(Nadine)


## Limitations
FOL is well suited to the description of [[Ontology|ontologies]] but:
	- FOL is rather verbose, therefore also rather bulky for modelling
	- difficult to achieve consensus in modelling
	- difficult to proof correctness and completeness of assertions
	 - It is not a Markup Language

To overcome these limitations, [[Description Logics]] have been introduced.


References:
[[Youtube - Semantic Web Technologies (L4)]]
[[Youtube - Semantic Web Technologies (L5)]]