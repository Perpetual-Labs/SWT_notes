Presented by [[Michael Uschold]]

Reasons to avoid silo:
 - lose meaning
 - no global IDs
 - not flexible
 - can't re-use schema

Purpose-built from start - don't pave cow paths
 - i.e. build in interoperability from start

Common schema used to avoid silos
 - can look like silos, but are actually interoperable
 - key enabler is URI for classes and properties

uses gist as TLO

Think big start small
 - large vision - we have
	 - Key deliverable - The Enterprise Ontology, cover max number of future domains with fewest concepts
	 - "Parti": high-level sketch or diagram of key concepts and relationships
 - start small - we are
	 - Key deliverable - demonstrate real value with real RDF data from at least two existing sources
	 - Build and populate knowledge graph - refine

collaborative workshops style approach

Reuse
 - Mostly borrow ideas - sometimes large chunks of OWL
 - To consider
	 - hierarchies of categories
	 - temporal relations (e.g. who is/was President)
 - Most reuse is reuse of ideas and patterns

Things to look out for
 - just a relational schema, presented in OWL
 - over-constraining domain and range
 - glorified taxonomies (no restrictions)
 - property proliferation (e.g. specific 'partOf' properties for each domain and range)
 - Class proliferation - becomes a glorified taxonomy

Style guide for gist
 - welcome to join and download from GitHub site
 - consider naming conventions: case, underscores, etc.

Include intermediate layer
 - separation of concerns
 - e.g.
	 - Ontology Layer: Country
	 - Taxonomy Layer: list of possible countries
	 - Data Layer: France
this point is useful for types - e.g. file type (.xlsx, .doc, etc.)

Things to check
 - e.g. is there a named inverse for a symmetric property?
 - more complex checks using SHACL
 - make sure have satisfactory checks in place
 - Check domain-dependent area - mostly runs queries in SHACL, sometimes SPARQL, to check
 - Libraries of queries called from scripts

Change management
 - What happens when a new version of an information artifact is released?
	 - consider ontologies, software,. Taxonomies., shapes
 - All about tracking dependencies
 - Must state dependencies in a triple
	 - e.g. version value must be between 2.3 and 3.0
 - Allow collections of items to be versioned together as one (e.g. group on ontologies)
 - Essentially, identify dependencies, have curators determine impact, and version up as necessary

## References:
[[Uschold2021 - Putting Enterprise ontologies into production]]