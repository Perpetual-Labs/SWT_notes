# Basic Formal Ontology:
developed by [[Barry Smith]]
Relatively simple [[ontology]]
It is a [[TLO]] like[[DOLCE]] and [[EMMO]]

![[BFO.jpg]]
![[BFO Top Layer.png]]
![[Independent Continuant Examples.png]]
![[Occurent Examples.png]]

## BFO Development:
 - This was developed from the [[Gene Ontology]]
 - The top three classes were inherited from GO and generalised
 - It has been applied succesfully in the [[OBO Foundry]]
 - It is being rolled out with the [[IOF]], chosen by [[NIST]]
 - BFO tries to build on scientific terminology, rather than cultural terminology (like [[DOLCE]])

## Future-Proof:
To future-proof an ontology:
 - rise up to a higher level of generality
 - e.g. like gene ontology - defined chemistry, not just human-specific stuff
 - then can be applied to all species

## Rules for Use:
 - see [[Ontology Rules]]

## Users of BFO:
 - ~300 ontologies use the BFO
 - [[NIST]] are big users
 - [[Barry Smith]] wants [[ST4SE]] to use BFO
 - https://basic-formal-ontology.org/users
 - in biology this has been used extensively and succesfully, see [[Smith2017 - Engineering Ontology Landscape]]

## Example of BFO and Domain
![[Jinzhi2020 - Knowledge graph modeling for decision-makings in the manufacturing systems.jpg]]
Reference: [[Jinzhi2020 - Towards Actionable Cognitive Digital Twins for Manufacturing]]

e.g. Aerospace is a domain of application for BFO

## BFO-2020 (BFO 2.1)
From 'What problem with OWL is BFO-2020 trying to solve'
[[Youtube2020 - What problem with OWL is BFO-2020 trying to solve]]

 - Problem with OWL treatment of relations
 - OWL does only binary relations - not ternary (i.e. composed of three parts)
 - so, no good for machines, wihich have parts that can be replaced.
 - e.g. saying 'Machine A has Part B' not the best way of doing it.
 - i.e. Part B might be replaced. So need a temporalised index of parts.

 - BFO 2 allowed people to use ternary as though binary - didn't solve problem
 - BFO 2.1 = BFO 2020
 - BFO 2.1 changes the way relations are treated

 - This problem arises between continuants and transitive properties (e.g. has-Part)
 - This is an issue when the parts change over time
 - so at instance level, it assumes the parts don't change

Very specific problem, can come back to if necessary




## Details - Terms:

Top-level breakdown:
 - Continuant:
	 - Independent Continuant
		 - maps to cellular component ([[Gene Ontology]])
		 - e.g. objects, parts systems
		 - Types:
			 - material entity
				 - object
				 - fiat_object_part
				 - object_aggregate
			 - immaterial entity
	 - Specifically Dependent Continuant
		 - maps to molecular function ([[Gene Ontology]])
		 - e.g. attributes, qualities, dispositions, roles, functions
		 - if object ceases to exist, then so does this
	 - Generically Dependent Continuant
		 - recent addition to BFO, used to represent 'information'
		 - must have a bearer, but does not need to be a specific one (i.e. copyability)
		 - e.g. PDF file on multiple laptops, DNA sequence in one chromosone
 - Occurent:
		 - maps to biological process ([[Gene Ontology]])
		 - e.g. processes, beginnings, endings, missions, operations
		 - these 'specifically_depend' on the independent continuant

e.g. Information Content Entity is a GDC (e.g. spacecraft design in a PDF), is concretised by an Information Quality Entity (e.g. physics of hard drive of laptop, a SDC), which is a qiality of the laptop.

Specifically dependent continuants:
 - quality (e.g. colour, temperature)
 - role (e.g. lawyer)
 - disposition (i.e. to do something)

Realisable dependent continuants:
 - are realised through processes
 - roles (externally realised through social processes)
 - dispositions (internally grounded realisable entity, e.g. side-effect of function)
 - Functions (raison d'etre of the object - realised by 'functionings')
 - non-realisable dependent continuant - quality

Must be careful about continuant and role differentiation.
 - e.g. a lawyer is not a continuant, it is a role - a human adopts that role for a given period of time


## Details - Physical places
 - fiat lines, surfaces, boundaries: not physcial boundaries but conceptual boundaries between sites
 - site: a 3D container
 - more detail on types of spaces, boundaries, regions, etc. provided in: [[Youtube - Introduction to BFO]]


## Details - Dispositions, Functions, Capabilities, Roles
Need to make distinction between having the ability to perform a function, and actually performing the function:
 - Disposition - internally grounded realisable entity
 - Capability - disposition whose realisation can bring benefit (to itself or to its user), and benefit can be graded.
   Depend on the context (may be beneficial in one context but not another)
   (not formally part of BFO yet)
 - Function - are the capabilities that we design the function for; the raison d'etre to the thing
 - Role - social agreement to realise a capability

Function (specifically dependent continuant):
 - e.g. to pump
Functioning (occurent):
 - e.g. pumping

## Details - Systems
Questions arise over where 'system' falls in the BFO.
Similar to 'object_aggregate'

Idea for definition of an engineered system:
an engineered system 's' is an aggregate of engineered artifacts a1, a2, ..., a_m
each of these artifcats has functions a_i:f_1 - a_i:f_n and capabilities
's' itself has function 'f', and exists because something was needed to realise function 'f', and is realised through the coordinated realisation of ai:f1 - ai:fn, and ai:c1 - ai:cn.

Hydraulic system example - upshot is: to understand the system, we need to understand its environment.
 - Examples of environment provided:
 - Biomes, ecological corridors, habitat, etc.
 - Taken from EnvO - the Environemntal Ontology (part of OBO Foundry)

Not sure of [[Barry Smith]]'s definition of a system:
 - Barry says: human is not a system
 - and washing machine is not a system.



References:
[[Standard - ISO,IEC PRF 21838-2.2 Information technology - Top-level ontologies (TLO) Part 2. Basic Formal Ontology (BFO)]]
[[Youtube - IOF. An ontology framework for the manufacturing industry]]
[[Youtube - Ontologies for Space and Ground Systems]]
[[Youtube - Introduction to BFO]]
[[Youtube - Ontology for SE Part 1. Introduction to Ontology]]
[[Youtube - Ontology for SE Part 2. Suites of Ontology Modules]]
[[Youtube - Ontology for SE Part 3. Functions and Capabilities]]
[[Youtube - Ontology for SE Part 4. Product Life Cycle]]
[[Youtube2019 - Ontology as Product-Service System A Study of GO, BFO and DOLCE]]