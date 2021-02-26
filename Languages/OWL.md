# Web Ontology Language - Overview

 - SHOIN(D), utilises OWA - see[[Description Logics]]
 - Developed by [[W3C]]
 - It is a semantic markup language for publishing and sharing ontologies on the web - developed as a vocabular extension of [[RDF]]
 - OWL Ontologies can therefore be exchanged as RDF documents
 - It is a [[Semantics|semantic]] Web language designed to represent rich and complex knowledge about things, groups of things, and relations between things.
 - It is a computational logic-based language such that knowledge expressed in OWL can be exploited by computer programs, e.g., to verify the consistency of that knowledge or to make implicit knowledge explicit.
 - It is the most widely used [[Knowledge Representation]] (KR) language in the world
- by a wide margin
- it is considered the accepted language
- It provides full [[Description Logics]] semantics (and beyond) and has powerful yet tractable reasoning [[Semantics]] - see [[Reasoners]]
- Used to define logical rules, e.g. LivingPeople and DeadPeople are disjunct classes - DeadPeople have the property DeathDate
- OWL provides a set of facilities to define domain-specific [[Ontology|ontologies]] in the context of the [[Semantic Web]]
- OWL Ontologies can be exchanged as RDF documents

# Main Concepts
 - [[Classes]]: define concepts and domains
 - [[Properties]] which are of two types:
		- Object properties: defined relationships between resources (URI)
		- Datatype properties: define relationships between a concept and a literal
- Individual instances of classes
- [[Constraints]] and [[Relations]] allow definition of cardinality restrictions as well as existential and universal quantifications


# Dialects
 - Multiple dialects available (e.g. [[OWL2]], OWL Lite) - see [[Blog2020 - Introduction to the Semantic Web]] for further info
 - OWL Lite (subsetOf) OWL DL (subsetOf) OWL Full

# Similar Languages
 - [[RDFS]] is on the same level as [[OWL]]
 - Describes classes (as opposed to level below, [[RDF]], which defines instances)

# Examples:
![[Example Ontology 1.png]]

![[Example Ontology 2.png]]



# References:
[[Jenkins - ST4SE]]
[[Youtube - Ontology for SE Part 1. Introduction to Ontology]]
[[Youtube - Semantic Web Technologies (L5)]]
[[Wiki - OWL]]










