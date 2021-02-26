# Official Title
RDF Schema
Officially: RDF Vocabulary Description Language

# Key Points
RDFS:
 - is a primitive [[Ontology]] language
 - is a universal model that lets users describe [[Resources]] using their own vocabularies
 - does not make assumptions about any particular application domain
 - does not define the [[Semantics]] of any domain
 - defines a data model for the creation of RDF statements
 - allows the user to define [[Classes]], [[Constraints]] and [[Relations]], etc.
 - It is up to the user to do so using an RDF Schema (RDFS) vocabulary.
 - i.e. it is a vocabulary description language for RDF with formal semantics.

# Purpose
 - RDFS does not provide a vocabulary of application-specific classes. Instead, it provides the facilities needed to describe such classes and properties, and to indicate which classes and properties are expected to be used together (for example, to say that the property JobTitle will be used in describing a class “Person”). In other words, RDF Schema provides a type system for RDF.
 - The RDFS facilities are themselves provided in the form of an RDF vocabulary, i.e., as a specialized set of predefined RDF resources with their own special meanings. The resources in the RDFS vocabulary have URIs with the prefix found at [[RDFSchema Repository]] (conventionally associated with the namespace prefix rdfs).
 - RDFS also provides facilities for describing how properties and classes are intended to be used together. The most important information of this kind is supplied by using the RDFS properties `rdfs:range` and `rdfs:domain` to further describe application-specific properties.

# Levels:
 - [[RDFS]] is on the same level as [[OWL]]
 - Describes classes (as opposed to level below, [[RDF]], which defines instances)
 - RDF is an instantiation of terminological knowledge (ontology) represented in RDF
 - T-Box:
	 - Terminological Knowledge (ontology, RDFS)
 - A-Box:
	 - Assertional Knowledge (instantiation, [[RDF]])

# Inferencing:
 - Can infer information based on the relationships provided (e.g. from [[SPARQL]])

# Example 1
![[RDFS Example.jpg]]

# Example 2
Example:
The `rdfs:range` property is used to indicate that the values of a particular property are members of a designated class. For example, to indicate that the property `ex:author` has values(objects) that are instances of class `ex:Person`, the following RDF statements are used:

	ex:Person   rdf:type     rdfs:Class .
	ex:author   rdf:type     rdf:Property .
	ex:author   rdfs:range   ex:Person .

These statements indicate that `ex:Person` is a class, `ex:author` is a property, and that RDF statements using the `ex:author` property have instances of `ex:Person` as objects.

The `rdfs:domain` property is used to indicate that a particular property is used to describe a specific class of objects. For example, to indicate that the property `ex:author` applies to instances of class `ex:Book`, the following RDF statements are used:

	ex:Book     rdf:type      rdfs:Class .
	ex:author   rdf:type      rdf:Property .
	ex:author   rdfs:domain   ex:Book .

These statements indicate that ex:Book is a class, ex:author is a property, and that RDF statements using the ex:author property have instances of ex:Book as subjects.


# References
[[Youtube - Semantic Web Technologies (L2)]]
[[Youtube2017 - RDF and OWL, Tara Raafat]]
[[RDFSchema Repository]]







