## Normal Form

### Definition

Parent + closest relationship


### Examples

Dog is a mammal that makesNoise some Bark

Human is a mammal that is childOf some Human


### Rector Normalisation

Also known as untangling

![[Normalisation.jpg]]


Can have multiple parents in the ABox
Multiple parents should not be asserted in the TBox
Multiple parents can be inferred in the TBox

So instead, you have two different 'isA' trees, and you link the two via an object property.


So, in the example below, left is tangled and right is untangled (normalised)

![[Normalisation Example.jpg]]


More complex example from the referenced paper is as follows:

![[Normalisation Example 2.jpg]]

### References
[[Rector2003 - Modularisation of Domain Ontologies Implemented in Description Logics and related formalisms including OWL]]