Open Services for Lifecycle Collaboration

an API standard to exchange data and [[Semantics]] using [[RDF]]-based languages and [[Ontology|ontologies]].

Goal:
 - "Achieve digital thread across domains, applications and organisations"				

Problem:
Pre-web	'Type 1' docs could not connect to 'Type 2' docs

[[Web History|Web (of docs)]]:
 - All docs are presented in [[HTML]], and are accessed using HTTP
 - Documents linked regardless of physical location			
[[Semantic Web|Web of Data]]				
	Represent data in [[RDF]], identified via [[URI]]s			
Note: I can definitely see the parallel paradigm shift - documents to models!				

e.g. Requirements Model:
 - OSLC --> [[RDF]] <--> [[DOORS]]
 - API standard
 - Use DOORS as Requirements and Database
 - Can use OSLC to connect to other tools 				
				
From Meeting - 201210:
 - OSLC uses syntactic vocabularies (in RDF)
 - not done in semantic way (i.e. not OWL)
 - So no inferencing - just linked data format
 - Focussed on tool integration at UI level (e.g. similar to [[Phoenix Integration - ModelCenter]]), not data level
 - [[OpenCAESAR]] is interconnected at a data level, not UI level (better)
 - Means that OSLC needs tool-specific adapters			
