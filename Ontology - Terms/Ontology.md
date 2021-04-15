# Overview
>People cannot share knowledge if they do not speak a common language"
\- Thomas Davenport 1997	

>An ontology is a formal, explicit specification of a shared conceptualization"
\- Tom Gruber 1992

Ontology: a knowledge model that defines allowable concepts and relationships within a domain

Metamodel: An explicit description of how a domain-specific model (following the rules of the ontology) can be built

"A valid metamodel is an ontology, but not all ontologies are modelled explicitly as metamodels"

To speak a common language means:
- common symbols and concepts (syntax)
- agreement aobut their meaning (semantics)
- Classification of concepts (taxonomy)
- Association and relations of concepts (Thesauri)
- Rules about which relations are allowed to make sense (Ontologies)

## Definition
Controlled vocabulary (collection of terms)
- Ontology supports automated reasoning and inference of the data using logical rules
- Provides knowledge sharing and re-using among people and software agents
- it goes one step forward from simply organising data in triples becuase it gives context to the data
- then use tagging to record whenever 'x' is mentioned all over the enterprise
- don't need to enforce a single language
- e.g. then can see if 'x' is tagged in multiple databases
- organisations (e.g. [[JPL]]) can have >100,000 databases
- Can then map between the ontology and a database (instance) by tagging (semi-automatically)
- ontology branches into defintions that are required and then mapped to the columns in the table
- e.g. no anatomy textbook of Bill Gates
	 - there is anatomy textbook (ontology) of a human
	 - and an instance (database) of Bill Gates

Note: Very few real-world examples of successful use of ontologies in engineering


## Levels
 - Level 1 - Triples (e.g. [[RDF]])
 - Level 2 - Ontology language (e.g. [[OWL]], [[RDFS]])
 - Level 2b - Ontology modelling languages (e.g. [[ORM]], [[OML]])
 - this then progresses to actual ontologies as below:

![[Knowledge Representation Layers.png]]

Ontology Levels:
 - Top-level: [[BFO]] (i.e. domain-neutral ontology)
    i.e. upper ontology, foundation ontology
	Defines 'Time', 'Space', 'Event', etc. (whole world)
 - Mid-level: [[CCO]], [[OBO Foundry]], [[IOF]]
 - Task-level:
    This may cover several domains.
	Fundamental concepts for a general activity / task
 - Domain-level: [[Space Domain Ontologies]]
    Fundamental concepts within a domain
 - Application-level:
   Specialised ontology focussed on a specific task and domain
 - Instance-level [[Knowledge Base]]: e.g. Biomass Spacecraft

## What is Ontology For?
 - to promote interoperability across heterogenous data systems
 - it does this by exploiting relative stability of natural language
 - HW and SW terms evolve rapidly
 - as opposed to a database - where they differ massively from enterprise to enterprise
 - once you have an ontology - you can map databases together
 - So you can't just base an ontology on your own database
 - just perpetuates the problem!
 - need to find a database-neutral level - very difficult to do
 - Ontologies serve as schemata or 'intelligent' views over information resources
 - Semantic repositories use ontologies as semantic schemata
 - This allows the data to be machine-processable, and therefore inferencing of facts which aren't directly stated (i.e. by [[Reasoning]])

## Current Problems:
 - Ontologies often fail
 - Too many, built independently, poor interoperability
 - Short half-life, poor documentation and training
 - Lack of commonly accepted standards
 - e.g. [[Linked Open Data (LOD)]] is an example of how bad it can get

## Applications
[[OBO Foundry]] generates biomedical ontologies (very successfully).
The [[IOF]] is used to generate ontologies for industry.
[[CCO]] is a collection of mid-level ontologies.
All of these are based on the [[BFO]].

## Key Definitions
- Formal = Machine readable
- Explicit specification = Meaning of all concepts must be defined. Entities, properties, relations, functions, constraints, axioms are explicitly defined
- shared =  consensual knowledge
- Conceptualization = Abstract model and simplified view of some phenomenon in the world that we want to present

## Ontology Types
Ontologies can be distinguished according to the sort of semantics being modelled and their intended usage:
Schema-ontologies:
 - Close in purpose and nature to database and object-oriented schemata
 - They define classes of objects, their properties and relationships to objects of other classes.
 - Typically involves using it as a vocabulary or glossary for defining large sets of instances.
 - In basic terms, a class in a schema ontology corresponds to a table in a relational database; a relation – to a column; an instance – to a row in the table for the corresponding class;
Topic-ontologies:
 - see [[Taxonomy|taxonomies]]
Lexical ontologies:
 - Lexicons with formal semantics that define lexical concepts.
 - A ‘lexical concept’ is a formal representation of the meaning of a word or a phrase.
 - e.g. semantic thesauri or dictionaries.
 - The concepts defined in such ontologies are not instantiated, rather they are directly used for reference

An [[Ontology]] can be classified as lightweight or heavyweight according to the complexity of the KR language and its expressivity:
Light-weight (informal) ontologies:
 - allow for more efficient and scalable reasoning
 - but do not possess the highly predictive (or restrictive) power of more powerful KR languages.
 - e.g. Vocabulary, terms, data dictionaries
 Heavyweight (formal) ontologies:
  - e.g. [[Description Logics]], [[First Order Logic]]


## Implementation Issues
 - Equivalence Mapping:
 - Some implementation issues can't be solved by [[OWL2 DL]] when combining multiple datasets
 - e.g. one model has 'FullName'
 - another has 'FirstName' and 'Surname'
 - another has 'FirstName' and 'LastName'
 - With [[OWL2 DL]] + [[SWRL]], we can say that 'Surname' = 'LastName' and map the two.
 - But, we can't use OWL2 to split 'FullName' into 'FirstName' and 'LastName'
 - So, OWL2 + SWRL may struggle to resolve more complex cases
 - Categorisation:
 - harder to explore design space than continuous and discrete
 - i.e. there is no 'direction' between the categories


## Ontology History
Ontology Timeline
-	1: 1970s: Strong AI, Robotics, PSL
	-	1970: robotics, Naive Physics, First Order Logic
	-	KIF: Knowledge interchange format (Tom Gruber... SIRI...)
	-	1985: Naive Physics Manifesto (patrick Hayes)
	-	1995: First Engineering Ontologies (all failed)
		-	A requirement ontology for engineering design (Lin, Fox, Bilgic)
		-	ontology as a requirements engineering product (Breitman)
		-	ontology-based active requirements engineering framework (lee gandhi)
	-	2003: Process specification lenguage (PSL) Ontology (Michael Gruninger, then NIST, Now Toronto). Exmaples: ISO18829 and ISO15926
		-	4 top level entities:
			-	Activity
			-	activity-occurence
			-	timepoint
			-	object
	-	They all failed: Typical reason for Fialure of engineering ontologies attempts in 2005:
		-	it was early days
		-	no common methodology
		-	short half-life (often funded by big public project, not really adopted by industry. stop to be maintained when funding runs out)
		-	approaches often tied to data modelling lenguages (UML, EXPRESS,...)
		-	no standard lenguage
		-	no documentation
-	2: 1990s: The Semantic Web, Linked Open Data:
	-	1994:  Tim-Berners-Lee introdcued the term "semnatic Web" at firs WWW Conference
	-	1994: Resource Descritpion Framework (RDF)
	-	1999: Protege'
	-	2004: Web Ontology Lenguage (OWL) 1.0
	-	Start of Ontology proliferation
	-	Linkd Open Data
	-	These has several advances over the previous phase (i.e. First Order Logic and PSL) but it sparked a proliferation of ontologies that created new problems: too many ontologies, all built differently, terminology bloat
-	3: 2000s: Lessons from the Human Genome Project
	-	1990: Human Genome Project
	-	1999: The Gene Ontology (GO): The first widely adopted ontology (both in accedemia and industry)
	-	2002: Open Biomedical Ontologies (OBO)
	-	Basic Formal Ontology (BFO)
	-	The reason why the GO succeeded (and the engineering ontologies of the 2000 fialed) is that it moved up one level of generality (abstraction) and this solved the half-short-life problem. It become super successfull in terms of users and volume of data.
-	4: 2005: The age of ontology suite.


## Ontology Rules
[[Ontology Rules|Rules]] also provided


References:
[[Blog2020 - Introduction to the Semantic Web]]
[[Youtube - IOF. An ontology framework for the manufacturing industry]]
[[Youtube - Ontology for SE Part 1. Introduction to Ontology]]
[[Youtube - Ontology for SE Part 2. Suites of Ontology Modules]]
[[Smith2017 - Engineering Ontology Landscape]]
[[Youtube - Ontologies for Space and Ground Systems]]
[[Youtube2017 - RDF and OWL, Tara Raafat]]
[[Youtube - Introduction to BFO]]
[[Youtube - Semantic Web Technologies (L4)]]