## Definition
Properties are a special kind of [[Resources|resource]]:
 - they describe relationships between resources
 - e.g., written by, age, title, and so on.
 - Properties in [[RDF]] are also identified by [[URI]]s (in most cases, these are actual URLs).
 - Therefore, properties themselves can be used as the subject in other statements, which allows for an expressive ways to describe properties
 - e.g., by defining property hierarchies.
 - Used to describe specific properties that characterise classes
 - e.g. numberOfBedrooms to describe an apartment
 - In [[RDFS]], properties are described using the [[RDF]] class rdf:Property, and the RDFS properties rdfs:domain, rdfs:range and rdfs:subPropertyOf.

## In RDF
All properties in RDF are described as instances of class rdf:Property. So, a new property, such as `exterms:weightInKg`, is defined with the following RDF statement:

	exterms:weightInKg   rdf:type   rdf:Property .

## Example Properties:
 - subClassOf
 - subPropertyOf (e.g. isMotherOf is a subproperty of isParentOf)
 - domain (property of a property)
 - range (property of a property)
 - See Example above
 - Other properties: seeAlso, isDefinedBy, comment, label



References:
[[Youtube - Semantic Web Technologies (L4)]]
[[Youtube - Semantic Web Technologies (L5)]]