# [[Ontology]] Rules

## General Principles:
 - Future-proof an ontology by modelling the ontology one level higher than necessary
 -  Start out from domain-neutral top-level ontology (hub and spoke approach)
 - Create suites of consistently developed ontology modules - with suite-wide oversight to ensure non-redundancy between modules
 - Define the terms used in ontologies
 - Rigourously enforce reuse of more general ontology content in more specific ontology resources (from reference ontologies to application ontologies)
 - Application ontologies are local ontologies
 - Key is to ensure local ontologies are built using same principles of reference ontologies
 - Then can infer information across the data of all applications
 - For A subClassOf B, define "A is a B that has this key difference"

![[subClass Example.png]]

 - Don't use Mappings - just have Reference Ontologies built around one or more single inheritance backbone taxonomies
 - Make domains modular - division of labour and authority
 - Avoid circularity
 - Make consistent with other ontologies (and e.g. dictionaries) to support computational enhancement of data - reduces need for mapping
 - Avoid 'Multiple Inheritance' (below), especially in reference ontologies - Do Diagram 2, not Diagram 1 (Single Inheritance only):
 - TBox - cannot have multiple inheritcance
    ABox - can have multiple inheritance
 - i.e. Terms should have at most one parent (this goes back to Aristotle)

![[Multiple Inheritance.jpg]]
![[Multiple Inheritance - Alternative.jpg]]

## [[BFO]] Rules
Never use mass nouns (e.g. information, sugar, luggage, knowledge)
 - must counteract 'silo syndrome' by making them interoperable with neighbours (must become part of BFO community fo ontologies)
 - must counteract 'half-life syndrome' by not starting with data (changes too quickly), but with the entities that the data are used to describe (i.e. objects, processes, etc.)
 - must counteract 're-invent the wheel syndrome' by following tried and tested methos:
   [[Standard - ISO,IEC PRF 21838-2.2 Information technology - Top-level ontologies (TLO) Part 2. Basic Formal Ontology (BFO)|ISO 21838]]
 - Domains come in nested stacks, and therefore so will domain ontologies
 - All-some rule: e.g. all brains are part of some head. Ontologies should only contain relations that follow the all-some rule. This is important because ontologies are not interested in instances. Only interested in meanings - and meanings should be universal


## Rules for terms:
 - Ontologies should be made up of general terms
 - But not all general terms correspond to 'universals'
 - i.e. do not create terms for universals through logical combination (e.g. brother of an Elvis fan)
 - this would be a 'defined class', not a 'universal'
 - links back to Single Inheritance, as above


## Ontology Components
Ontologies may include information such as:
 - [[Classes]] (e.g. all managers, c, are also staff members, c')
 - [[Properties]] (e.g. x is subordinated y)
 - [[Constraints]] and [[Relations]], [[Values|Value]] Restrictions (e.g. only managers may head departments)
 - Disjointness statements (e.g. managers and general employess are disjoint)
 - Specifications of logical relationships between objects (every department must have at least three staff members)
 - and how properties and classes are intended to be used together. (e.g., an object which has property Hasprice is a member of the class Products)
An ontology, o, can therefore be defined as comprising the 4-tuple:
	o = <C, R, I, A>	
where:
 - C is a is a set of classes representing concepts from the domain we wish to describe (e.g., invoices, payments, products, prices, etc);
 - R is a set of relations (also referred to as properties or predicates) holding between (instances of) these classes (e.g., Product hasPrice Price);
 - I is a set of instances, where each instance can be a member of one or more classes and can be linked to other instances or to literal values (strings, numbers and other data-types) by relations
 - A is a set of axioms (e.g., if a product has a price greater than €200, then shipping is free).	

![[Ontology Definitions.jpg]]


## Sharing Vocabularies:
[[RDFS]] provides the means to create custom vocabularies.
 - However, it is generally easier and better practice to use an existing vocabulary that describes a similar conceptual domain.
 - Such publicly available vocabularies, called ‘shared vocabularies’, are cost-efficient to use and promote the shared understanding of the domains.
 - The use of [[URI]]s does not solve all identification problems, because different URIs can be created for referring to the same thing. For this reason, it is a good idea to have a preference towards using terms from existing vocabularies.
 - e.g. [[Dublin Core]]
 - Appropriate vocabularies for use in specific application areas are being developed all the time, but even so, the sharing of these vocabularies in a common ‘Web space’ provides the opportunity to identify and deal with any equivalent terminology.


References:
[[Blog2020 - Introduction to the Semantic Web]]
[[Youtube - IOF. An ontology framework for the manufacturing industry]]
[[Youtube - Ontology for SE Part 1. Introduction to Ontology]]
[[Youtube - Ontology for SE Part 3. Functions and Capabilities]]
[[Smith2017 - Engineering Ontology Landscape]]
[[Youtube - Ontologies for Space and Ground Systems]]
[[Youtube - Introduction to BFO]]