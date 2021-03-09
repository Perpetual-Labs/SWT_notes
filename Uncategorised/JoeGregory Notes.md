
Don't organise until Gian has provided me with the Git Repo

3.8 EXTRA Protege Demo
https://www.youtube.com/watch?v=m1Xcn5nUhdA&ab_channel=OpenHPITutorials
Add reference to OWL detail rules, or Protege page
Also add the other Protege demos I have watched.
https://www.youtube.com/watch?v=akz0Me7Mdmg&t=490s&ab_channel=AmirIdris
https://www.youtube.com/watch?v=R9ERlUgvgwM&list=PLea0WJq13cnAfCC0azrCyquCN_tPelJN1&ab_channel=NoureddinSadawi


Monday 8th

Protege experimentation
Downloaded VOWL and got working
Familiarised with OntoGraf (this is better than VOWL)
Produced SEAM Ontology v2
Includes all classes, object properties and data properties
Made a start on the instances
Made some changes to SEAM Ontology
 - Added mission entities
 - Added 'SystemOfInterest' and the LogicalSystem represents this
 - TopFunctions satisfy Capabilities
 - Functional Chains are made up of LowerFunctions (i.e. not TopFunctions)
 - Added 'Cluster' concept as a collection of functions
 - Removed 'Clustering' process for Components - they are produced by some other process
 - Added 'withRespectTo AstronomicalBody' for 'Position'
 - Added intermediate classes- Mission, Operations, System (Functional, Logical)

FOund these references
UML to OWL Reference:
https://henrietteharmse.com/uml-vs-owl/uml-class-diagram-to-owl-and-sroiq-reference/
https://henrietteharmse.com/wp-content/uploads/2017/11/uml-class-diagram-to-owl-and-sroiq-reference.pdf
OWL 2 Primer:
https://www.w3.org/TR/2012/REC-owl2-primer-20121211/
Series of short Protege tutorials:
https://www.youtube.com/watch?v=QY9M_j2Ta14&list=PLea0WJq13cnAfCC0azrCyquCN_tPelJN1&index=6&ab_channel=NoureddinSadawi



Gian Meeting - 210216

2 Uni of Newcastle Students
Working on Biomass stuff
Experts in co-simulation, uncertainty quantification, surrogate modelling



OntoCommons Meeting Prep:

Ontocommons - ontology-driven data documentation for industry commons

Dedicated to standardisation of data documentation across all domains related to materials and manufacturing

FACTLOG - real-time procssing layer, sits between digital twin (domain model) and real-time data model (i.e. from observation)




Paper: Towards Actionable Cognitive Digital Twins for  
Manufacturing

Cognitive Twin: Digital Twin + behaviour (i.e. make DT actionable) + Knowledge Graph (instantiation of ontology)

behaviour: decision-making algorithms, real-time processing of data

Fig 2. BFO and Domain

Problem 1: Anomalies

Problem 2: Production planning

Questions:

Is the BFO the only pre-defined ontology you used? E.g. 'Information Content Entity' could already exist?

How many relationships (object properties) are defined between the classes?

Where is 'actionable' part?





Paper: Systems Engineering Approach to Identify Requirements for Digital Twins Development

However, the DT concepts are separately defined by different domains, which leads to challenges defining a unified DT concept.

ISO 42010 concluded that most of the key  
concepts and meta-models in different architectural knowledge management  
(AKM) tools are consistent.

ISO 42010 can xupport DT architectur descriptions

Reference architecture in here is useful

Used ISO 42010 and EARS Approach to define the viewpoints necessary in the architecture

Identifies key decision-making capabilities of the DT

Questions:

Can a DT be applied to a logical model? Or does it have to be physical?

So this a method for developing key requirements of the DR itself?





Paper: Model-Based Systems Engineering Tool-Chain for  
Automated Parameter Value Selection

The existing works show that MBSE and tool-chains are  
widely used for CPS development. 

However, most of them  
were developed for specific purposes, limiting further extension.

DSML is neccesary to capture particular modelling featrues

Interoperability between tools

Really good template for the kind of work I've done

Look at Tables 3, 4, 5, see if there's anything I could do like this

Model Structure

System configuration (and behaviour?) model

simulation parameters model

Decision-making model

i.e. so simulate multile configurations and automatically choose the best one






Paper: Cognitive Twins for Supporting Decision-  
Makings of Internet of Things Systems

Cognitive Twin: DT timestamped through every life cycle phase (evolution of system), and ontology of relationships

CTs are used for dynamic process simulation

Key part is the relationships between the models themselves (ontopology)

e.g. requirements models, decision-making models, etc.

Ontocommons:

Top Reference Ontology (TRO) - relation to BFO?

What is the status of the SE Ontology? (would that be a middle level ontology? (MLO)

What is the process for getting involved? E.g. how do we find overlap?

Is the BFO the only pre-defined ontology you used in your Actionable CT paper? E.g. 'Information Content Entity' could already exist?





OntoCommons Meeting - 210215
      
Dmitris - co-founder of IOF
2016 - met Barry Smith
launched IOF together

Aerospace is a domain of application for these technologies

Airbus want to use ontologies in MBSE - but in quality

starting with SE, moving on to MBSE

IOF - registered by April/May (legal entity)
autonomous part of AOGI
OntoCommons - standardisation activities with a couple of ISO committees

David Cameron - chemical engineer, now 5 years in academia
Digital Twins research at Uni of Oslo

Hedi Karray - technical manager of OntoCommons
Professor at EMITS, Toulouse
OntoCommons ToolKit - guidelines, methodology, tools, etc.

Gian interested in discussing possible collaborations 

Presentation on OntoCommons to follow:
 - Overcome interoprability bottlenecks
 - Coordination and Support Action (CSA)
 - Ontology Commons Ecosystems (OCES) as foundation
 - Starts with TLO
 - Tools and specs for building ontologies and data documentation
 - no standardised tools / methodologies
	 - intra- and cross-domain interoperability
 - deliver a number of demonstration cases
 - Process:
1: Community development (i.e. involve stakeholders, etc.)
2: OCES (to facilitate development of domain ontologies)
3: Demonstrators (case studies)
Eleven use cases already
engaged to have ten more

Not one TLO
Have a Top Reference Ontology (TRO)
Then a Meta Ontology (MO)
Then multiple TLOs (e.g. BFO, DOLCE, EMMO)
enables alignment between e.g. BFO and DOLCE
Semantic and syntactic alignment

How is the BFO and EMMO on the same level?

MT Connect - standard to enable sharing of data between machines and tools

Dmitris: use ontology for DTs and CTs
Focussed on requirements for now
not quality processes - like Gian is interested in

Gian - Ciphre and MBQP

Dmitris: very good that Antonio is looking to connect with people in Toulouse re: ontologies
 - Align the two processes
 - Allow Antonio and people in Toulouse to find each other and discuss
 - Perpetual Labs - now part of the CSA community
	 - will be invited to join formally - then can be invited to workshops
	 - can submit our own demonstrator if we want
 - Align the wants of the Airbus ontology and our ontologies

 - How do we start to learn about technical and practical tools?
 - Workshops in March - workshop on demonstrators 9/10 March
 - workshop 15 March - domain ontologies
 - outcomes of workshop - define domains, collect ontology requirements from stakeholders
 - 19 March - workshop on ontology tools
 - after this - create expert groups
 - then develop hierarchy of ontologies

Dolce is another example of a TLO
 - BFO is not the truth! It's one philosophical vision of an ontology
 - different philosophical visions of ontologies
 - so terminological and syntactis alignment
 - TRO - align branches of ontologies 
 - maybe more of a mapping between terms?

So - OntoCommons are developing SE ontology (domain)
and have demonstrators lined up
we should learn from this and then contribute back to workshops
OntoCommons will be built on ISO standards (e.g. look up 59260)
so it will be an iterative process
For now, I can try and get the SEAM to map to the BFO
Ontology can be used to describe the model content - rather than just the system
ontology is a static representation of reality
Objective is to represent the real world and its dynamics accurately - across any graphical representation and language

Languages:
BFO and IOF, must be in English and OWL, FOL
IOF and OntoCommons will both be compatible with OWL DL (ISO, W3C standard)
Will incorporate processes - discrete and continuous
 - but to have actionable processes - ontology cannot do this - need to transfer to e.g. SysML

e.g. the term 'optimisation' is not in the ontology, it is defined later in the tool
ontology doesn't capture dynamic so far
some examples of trying to capture this other kind of stuff (ICS OWL - French group tries to capture equations)

UoM, participating in OntoCommons through University of Oslo
OntoCommons - not aware or linked to OSMOSE
Perpetual can make the link

Damiano Arena (EPFL) - look for papers
Also look up Farhad Ameri

Autodesk Toronto - involved in IOF
Jim Logan (MagicDraw) now involved in IOF
Chris Wild (Appraiso) also bought by Dassault Systemes

Tools:
Recommendation: Stick with Protégé
Readi (academic-indudtry tool? Focusses on requirements. Look this up)

Academic network re: requirements - 
INTOCPS

![[IOF Systems Engineering Roadmap.png]]

Links to - and descriptions of:
ISO 15288
ISO 42010
ISO 29148
ISO 24765



Youtube: What problem with OWL does BFO 2020 solve?
add link and reference note to 'Resources - Reviewed' folder and the Vault when I have the latest version.

Problem with OWL treatment of relations
OWL does only binary relations - not ternary (i.e. composed of three parts)
so, no good for machines, wihich have parts that can be replaced.
e.g. saying 'Machine A has Part B' not the best way of doing it.
i.e. Part B might be replaced. So need a temporalised index of parts.

BFO 2 allowed people to use ternary as though binary - didn't solve problem
BFO 2.1 = BFO 2020
BFO 2.1 changes the way relations are treated

This problem arises between continuants.
and transitive properties (e.g. has-Part)
This is an issue when the parts change over time
 - so at instance level, it assumes the parts don't change

Very specific problem, can come back to if necessary



Ontology as Product-Service System: A Study of GO, BFO and DOLCE
Youtube - as above

NIST - decision procedure to determine which ontology should be TLO for IOF.
Evaluated BFO against DOLCE in 43 dimensions
DOLCE is based on cultural (e.g. natural language and human common sense, social conventions)
BFO tries to build instead on scientific terminology
Therefore, there are lots of variants - only one official one (2002)
This is not a good approach to ontology - people shouldn't create their own versions.
DOLCE has one good application in Hydrology, but others are not so good
 - e.g. developed independently, can't be tracked online, etc.



210222 - Gian, Omar meeting

PL Projects:
MBQP: Boeing - SE for manufacturing
Ciphre: Airbus (Antonio), BAE, IBM - open-ended

Thierry Chavalier meeting outcomes:
use of ontology - Thierry not fuly convinced, but perhaps he was thinking more of a controlled human vocabulary
ISO 81346 (RDS) - This is used at the moment, information is tagged. Look into

Stardog:
Semantic web, knowledge graph people
Big renaissance in semantic web in the last couple of years
SHAQL - standard around it (e.g. as OWL is SHROIQ(D))
Shapes constraint language

Issue of Ontology:
Difference between SE system decomposition and decomposition for simulation
i.e. different stakeholders view system in different ways
Thierry feedback: this is more difficult than PL has assumed
Essentially, need to cater to different architecture viewpoints
e.g. 100 papers - structured by author, date and topic


TBox - cannot have multiple inheritcance
ABox - can have multiple inheritance

Some implementation issues can't be solved by OWL2 when combining multiple datasets
e.g. one model has 'FullName'
another has 'FirstName' and 'Surname'
another has 'FirstName' and 'LastName'
with OWL2 + SWRL, we can say that 'Surname' = 'LastName' and map the two.
But - we can't use OWL2 to split 'FullName' into 'FirstName' and 'LastName'
So, OWL2 + SWRL may struggle to resolve more complex cases

Other issues to consider:
Categorisation
 - harder to explore design space than continuous and discrete
 - i.e. there is no 'direction' between the categories
 - Omar to look into (provide an overview of how to deal with)
Uncertainty Quantification (QUTE)
 - Gian to look into this
Co-simulation
 - INTO-CPS will help to solve this
 - Gian to look into this



210222 - Barry Smith Meeting

Involved in two organisations:
CUBRC
 - military focus in Buffalo
 - Air Force Research Lab, interest in MBSE
 - not really interested in making work with SE software
 - Barry to provide contact, but we need to tread carefully when talking with them
IOF
 - Airbus are one of the quasi-members (no members yet as free due to Covid)
 - Barry recommended contacting Airbus contact (Barry to provide)
 - Systems Engineering WG
	 - one of us to join
	 - 1 hour every two weeks
	 - OntoCommons overlaps woth SE WG (but is relatively new)
	 - Ideally, would like OntoCommons to take over the WG.
 - MTConnect WG
	 - sensor data in factories
	 - maybe relevant to cars, spacecraft, etc.
 - Interoperability WG
	 - ensures the WGs work together
	 - key is that they all use BFO

IOF Overview
 - MLOs, Common Core Ontologies
 - CCOs use Common Logic (basically FOL)
 - OWL Logic is used in the CCO models (Description Logics)
 - we can contribute by developing an ontology that fits in here

Modelling and SImulation
 - no WG yet, but would like to kick off
 - CUBRC are interested in Digital Twin modelling
 - Autodesk Toronto - working on ontology for Modelling and SImulation
 - Barry to provide name of contact





ESA OSMOSE - Executive Summary Report
add to References when have access to Repo

Solution to address interoperability at semantic level:
Information modelling at system specification level
i.e. Build a global conceptual data model for the Space System - the Space System Ontology

Space System Ontology governed by two groups:
 - Management Steering Group (MB4SE Advisory Group)
 - Design Authority Group (OSMOSE WG)

Relevant documents:
Steering Group Terms of Reference
Design Authority Group Terms of Reference

Project Plan:
Four groups of stakeholders:
 - Ontology governors (control ontology development)
 - Ontology developers (develop the ontology)
 - Interoperability developers (enable interoperability at physical level)
 - Users (apply ontology though tools that enforce interoperability)
Details the principles that guide development
 - Development policy
 - Dissemination plan
 - Quality and product assurance
 - Programme of work
Defines the use cases that shall be considered during the ontology definition
- Inspired from ECSS-E-ST-10C
- Organised according to SE activities
- Chosen to allow identification of terms of interest

Development Plan:
Scope and priorities of the ontology:
 - Ontology shall address system aspects of any space systems
 - Its scope is limited to the engineering data
 - It shall focus on what is exchanged, and detail requied
 - It shall model generic elements at system level
 - These generic elements shall later be instantiated in different domains
The development plan is based on 8 Universes of Discourse
1. Requirements management
2. Mission and operation
3. Functional description of the static view
4. Functional description of the behavioral/dynamic view
5. Logical description
6. Physical description
7. Managing and planning
8. Support to config control, CM and NC control

Tools, Languages:
These UoDs will be conceptualised using ORM and NORMA Pro.
Then use translation tools to automatically generate e.g. UML, Ecore, XML

OSMOSE WG Outputs:
The ORM model of the SSO



https://www.researchgate.net/publication/320148742_Ontology-based_Knowledge_Management_for_Space_Data
Rovetta2017

This mainly focusses on space science data, rather than the systems themselves

Ontology engineering: the set of activities that concern the ontology development process, the ontology life cycle, the methods and methodologies for building ontologies, and the tool suites and languages that support them

Review of Ontology in astronautics and the space sciences:
 - Orbital Space Domain Ontology Project (by author)
	 - Orbital Debris Ontology (ODO)
	 - Space Situational Awareness Ontology (SSAO)
 - NASA Semantic Web for Earth and Environmental Terminology (SWEET)
	 - ~6000 category termst
 - Ontology-Driven Interactive Search ENvironment for Earth Sciences (ODISEES)
 - NASA Planetary Data System (PDS)
	 - archive of data and metadata for planetary science
 - ESA Earth Observation (EO) Knowledge Navigational System
	 - knowledge management system for EO imagery
 - IVOA Ontology of Astronomical Object Types
 - Space Surveillance XML Schema
 - NASA Exploration Initiatives Ontology Models (NExIOM)
	 - semantic approach to knowledge reuse within NASA
 - NASA Quantities, Units, Dimensions and Data Type (QUDT) Ontologies
 - International Space Station Schema
 - XML Capability Analysis Library (XCALIBR)
	 - spacecraft ontology for 'plu and play' assembly of spacecraft
	 - focusses on spacecraft components
 - ProjectChronos
	 - Developed RDF ontologies of aerospace engineering concepts, systems and subsystems, astronomical objects, etc.
 - USOC's Knowledge Integration and dissemination for Space Science and Exploration (ULISSE)
 - State Analysis Ontology
	 - Fundamental concepts and control system concepts
	 - Maps from ontology to SysML elements
 - Ontology of the functions of SPICE
	 - Erica Wick
 - Mars Rover Ontology for tele-robotic science
	 - Wales, Shalin, Bass



ESA Space System Ontology Workshop Presentations

1. Space System Ontology - Wlecome

