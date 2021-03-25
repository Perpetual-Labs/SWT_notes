# Definition
A class is a special kind of [[Resources|resource]] that can be thought of as a set of elements.
 - Top-level class is a resource
 - Other examples include: Property, Literal, Datatype, XMLLiteral, Container, ContainerMembershipProperty
 - Represent concepts
 - Described via [[Attributes]]
 - Defined with a capital letter, e.g. 'Person'

# Detail
 - Individual objects that belong to a class are referred to as instances of that class.
 - A class in [[RDFS]] corresponds to the generic concept of a type or category similar to the notion of a class in object-oriented programming languages such as Java.
 - [[RDF]] classes can be used to represent any category of object such as web pages, people, document types, databases or abstract concepts.
 - Classes are described using the RDF Schema resources rdfs:Class and rdfs:Resource, and the properties rdf:type and rdfs:subClassOf.
 - The relationship between instances and classes in RDF is defined using rdf:type.

An important use of classes is to impose [[Constraints]] and [[Relations]] on what can be stated in an RDF document using the schema:
 - In programming languages, typing is used to prevent incorrect use of objects ([[Resources]])
 - The same is true in RDF imposing a restriction on the objects to which the property can be applied.
 - In logical terms, this is a restriction on the domain of the [[Properties|property]].


References:
[[Youtube - Semantic Web Technologies (L5)]]