# Definition of Terms
[[Resources]]:
 - must be referenced by [[URI]]
Description:
 - describes resources using [[Properties]] and [[Constraints]] and [[Relations]] represented as graphs
Framework:
 - combination of web-based protocols ([[URI]], HTTP), based on formal model ([[Semantics]]), defining all allowable relationships among resources
Although frequently referred to as a ‘language’, RDF is mainly a data model.

# Purpose
 - Enables intuitive [[Knowledge Representation]] with directed graphs (i.e. [[Knowledge Graph]])
 - Schema-free
 - XML compatible for ease of data exchange
 - RDF does not make assumptions about any particular application domain, nor does it define the semantics of any domain. It is up to the user to do so using a domain-specific "vocabulary" such as the [[Dublin Core]] which is defined using a appropriate vocabulary lenguage such as [[RDFS]]. As can be see from the example above, a dimain-specific "vocabulary"  which defines the property `has creator` is necessary to give meaing to the triple. Formal [[Ontology|ontologies]] can be used as a form of domain-specific vocabularies.

# Levels
 - 1: Objects ([[XML]], XMLSchema)
 - 2: Knowledge ([[RDF]], [[RDFS]])
 - 3: Entire worlds ([[OWL]])
 - RDF describes instances (as opposed to level above, which describes [[Classes]])

# RDF Triples:
- Resource (URI) has a Property (URI) which has a Object (URI) / [[Values|Value]] (Literal)
- Resources and properties represented by [[URI]]s
- Subject - Predicate - Object
- Resource - Property - Resource(URI)/Value(Literal)

# RDF Representations:
Node-Edge-Node:
	 - graph representation
N3: code representation
	 - three parts separated by commas
Turtle (Terse RDF Triple Language)
	 - Extension of N3
	 - URIs in angle brackets
	 - Literals in quotation marks
	 - Triples closed with a period
	 - Can define prefixes for common URIs
RDF XML Serialization
	 - this is the standard
	 - longer than Turtle

Examples provided throughout [[Youtube - Semantic Web Technologies (L2)]] in Turtle and RDF XML Serialization, including:
 - Fragment identifiers
 - Base prefixes
 - Multi-valued relations (e.g. lecture in two rooms)
 - Blank nodes (Bnodes)
 - Lists (sequential containers, bags, alternatives, collections) - no semantic meaning, just convenient
 - Reification (statements abouts statements)
 - Data integration (combining multiple graphs)


# Example
To make the information in the following sentence
> “The web site www.johndoesite.com is created by John Doe.”

machine-accessible, it should be expressed in the form of an RDF statement, i.e., a subject-predicate-object triple:

	[subject] the web site www.johndoesite.com [predicate] has a creator [object] called John Doe.

The RDF statement above could be represented by the following graph:
![[RDF Graph Example.png]]
This kind of graph is known in the artificial intelligence community as a ‘semantic net’.



# References
[[Blog2020 - Introduction to the Semantic Web]]
[[Youtube - Semantic Web Technologies (L2)]]
[[Youtube2017 - RDF and OWL, Tara Raafat]]
[[Youtube2011 - The Semantic Web-An Overview]]


