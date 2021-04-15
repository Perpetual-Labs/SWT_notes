When building an [[Ontology]], there can be multiple models of the same world.

Therewere we need:

## Ontological Engineering
Ontology Design
 - Methods for efficient development of ontologies
Ontology Mapping
 - Methods for efficient comparison of ontologies
Ontology Merging
 - Methods for efficient merging of ontologies

Need methodologies of ontology deisgn
 - to make consistent
 - to do efficiently
 - to produce distributed development of ontologies
 - Involves: scheduling, control and QA

Ontology engineering: the set of activities that concern the ontology development process, the ontology life cycle, the methods and methodologies for building ontologies, and the tool suites and languages that support them

## Steps:
1. Pre-development
	1.	Environment study (software and applications)
	2.	Feasibility study (is it possible?)
2.	Development
	1.	Specification (what is its purpose, stakeholders?)
	2.	Conceptualisation (structure domain knowledge into conceptual model)
	3.	Formalisation (formalise conceptual model - semi-computable)
	4.	Implementation (construction of computable model)
3.	Post-Development
	1.	Maintenance (Update and adjust the ontology)
	2.	Use / Reuse (Use it in planned and unplanned applications)

## Ontology support activities:
 - Knowledge Acquisition (Ontology learning)
 - Evaluation
 - Integration (Ontoloy reuse)
 - Merging
 - Alignment (e.g. mapping rules)
 - Documentation (i.e. of the development process)
 - Configuration Management (of Ontology and documentation)

## Verification, Testing
from [[OntoCommons]] Workshop
 - Error provokation
 - Inference verification
 - CQ testing
(Arco tutorials available on YouTube)

[[Juan Sequeda]]:
Test-driven development:
 - Catalog validity tests
 - Ontology coverage tests
 - [[SHACL]] coverage tests
These activities all support each other

[[Michael Gruninger]]:
Actual ontology models = 
some intended models (but some ommitted) + some unintended models
Verification of ontologies checks these subsets

Instance verification, example by Gianmaria:
A component is required to have three interfaces
If an instance of a component has only two defined, the reasoner will flag this missing interface as an error


## Noy Process
(see reference)
1. Determine scope
2. Consider reuse
3. Enumerate terms
4. Define classes
5. Define properties
6. Define constraints (e.g. cardinality, data types)
7. Define axioms
8. Create instances

It is an iterative process - sometimes need to go back
There is no one way to model a domain - there are always viable alternatives
Basically just an application of of the methodology discussed above


## Orellana Process
1 - Scope the Ontology
 - Purpose of ontology, who will be using.
 - Interviews with Subject Matter Experts
2 Establish a Lexicon
 - Identify high-frequency terms that will make up the classes and properties
3 Map to [[TLO]]
 - e.g. [[BFO]]
 - Creates the taxonomical hierarchies
4 Establish [[Axioms]]
 - Creates the horizontal (axiomatic) relationships
 - Establish as many as possible to increase power of [[Reasoning]]
5 Populate with Instances
 - i.e. Case Study data (e.g. [[LAST]])


References:
[[Youtube - Semantic Web Technologies (L6)]]
[[Rajpathak2011 - A generic ontology development framework for data integration and decision support in a distributed environment]]
[[Noy2005 - Ontology Development 101]]
[[Rovetto2017 - Ontology-based Knowledge Management for Space Data]]
[[orell]]
[[Orellana2019 - The Ontology of Systems Engineering. Towards a Computational Digital Engineering Semantic Framework]]