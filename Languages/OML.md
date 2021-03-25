# Ontological Modeling Language
Used to model [[Ontology|ontologies]]
Developed by [[JPL]] for [[ST4SE]]
Part of [[CAESAR]], led by [[Maged Elaasar]]

## Features:
 - Tool-neutral representation
 - Supports queries and query languages (e.g. [[SPARQL]])
 - Abstractions are: vocabulary & modelling
 - Can link multiple OML models together - can't do that in UML really		
 - So can fragment into libraries, store in repositories, and use a Git system to develop
 - This means you can do your modelling like programming	

## OWL Relationship:
 - Designed after [[OWL]] (specifically [[OWL2 DL]])
 - Consider as profile
 - OML is a thin vocbaulary extension to OWL2 to support SE models
 - OWL maps to SysML, therefore so does OML
 - Think of OML as a methodology of using OWL
 - An OML Module maps to an OWL2-DL Ontology with SWRL rules both structurally and semantically.
 - An [[OWL2 DL]] Ontology provides classes, properties, individuals and data values that are represented in Semantic Web documents.
 - These constructs form the basis of the OWL2-DL+[[SWRL]] mapping of an OML Module whose corresponding constructs include OML Entity, OML EntityRelationship, OML Datatype, OML DataProperty and OML TerminologyInstanceAssertion.

## From [[Steven Jenkins]]
 - OML captures ~24 [[OWL]] patterns, specifically highly mapped to [[OWL2 DL]]
 - e.g. [[OWL]] struggles to handle reification with [[RDF]] triples.


## Bundles:
 - OML bundle maps corresponds to modeling language metamodel
 - provides an ontology for a particular world - but world is kept open (extensible)

## Tools:
 - [[JPL]] use [[Eclipse]] platform, [[Rosetta]] (and xtext)		

## Analytical stuff:
 - Define vocabularies and interfaces to analytical models
 - Need behaviour defined in a certain way - as an OML ontology
 - Semantic, vocab-based interfaces mean data can be fed into simulation engines
 - [[Maged Elaasar]] recommended that this would be a good place for us to work.




References:
[[GitBooks - OML Specification]]