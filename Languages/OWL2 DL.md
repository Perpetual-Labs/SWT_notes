# OWL 2

OWL EL, OWL RL, OWL QL
 - are (subsetsOf) OWL 2 DL
 - which is a (subsetOf) OWL 2 Full

**In this the focus is mainly on OWL 2 DL**
 - SHROIQ(D)
 - utilises OWA
 - utilises 'No Unique Name' assumption
 - see [[Description Logics]]
 - [[W3C]] Recommendation since 2009

## OWL 2 DL Overview
The [[Description Logics]] subset of [[OWL]]
 - carefully chosen to balance expressivitiy (i.e. richer [[Semantics]]) with computational complexity of [[Reasoning]]
 - In particular, practical reasoning algorithms exist that are both:
	- sound: all inferences drawn are valid
	- complete: all valid inferences are drawn
 - These algorithms have been implemented in both commercial and free software that is widely used
 - In addition, these reasoners can detect various errors such as inconsistencies or unsatisfiable (i.e., overconstrained) classes
 - Information expressed in OWL can be semantically validated
	- We have an opportunity to catch errors on every exchange

## OWL 2 DL Details
See [[W3C - OWL 2 Primer]]

Subset of [[OWL2 DL]]
SHROIQ(D)

### SHROIQ(D)
S: ALC + Transivity of roles
 - if aRb and bRc, then aRc (e.g. isAncestorOf)
H: Role hierarchies
 - R subpropertyOf S
R: Role constructors
O: Nominals
I: Inverse Roles
Q: Qualified number restrictions <nR.C etc.
(D): Datatypes

![[DL Conventional Notation.jpg]]

Class constructors:
 -conjunction (and) (∧)
 -disjunction (or)(∨)
 -negation (not) (¬)
Property restrictions:
 -Existential, Ǝ, property restrictions
 -Universal, ∀, property restrictions
Number restrictions:
  -"<n R"
Closed classes (nominals):
 -{a} (O)

### Syntax Variants
Functional syntax:
- easy to define, no RDF restrictions, more compact
RDF-Syntax:
- important for compatibility issues
- but more complex
XML-Syntax:
- similar to above
Manchester-Syntax:
- machine-readable syntax
Turtle:
- most simple and easy to write
- examples provided herein use Turtle


### OWL Reminder
OWL:
 - Classes, inviduals, properties
RDFS:
 - Classes, objects, properties

Two OWL predefined classes:
 - owl: Thing (class that contains all individuals, Top)
 - owl: Nothing (empty class, Bottom)

### Prefixes
To access predefined classes and properties:
Access 'Prefixes and Namespaces'
dc:      <http://purl.org/dc/elements/1.1/>
grddl:  <http://www.w3.org/2003/g/data-view#>
owl: 	 <http://www.w3.org/2002/07/owl#>
rdf: 	  <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
rdfs:	 <http://www.w3.org/2000/01/rdf-schema#>
xml: 	 <http://www.w3.org/XML/1998/namespace>
xsd:     <http://www.w3.org/2001/XMLSchema#>


### Examples

#### Definition of a class, e.g:
 `:Wine a owl:Class`
Definition of an individual, e,g:
`:WegelerRhengauRiesling a :Wine`
Individuals can also be defined without direct class membership as "named entity":
`:JoeGregory a owl:NamedIndividual`
OWA means that the class that JoeGregory belongs to can be added later

#### OWL - Properties:
Object properties, defined like classes, e,g:
`:isMadeFrom a owl:ObjectProperty`
and can restrict domain and range, e.g:
`:isMadeOf  a owl:ObjectProperty ;`
`rdfs:domain  :Wine ;`
`rdfs:range     :Grapes .`
Datatype Properties, e,g:
`:hasVintageYear a owl:DatatypeProperty .`
and can restrict domain and range, e.g.
`:hasVintageYear a owl:ObjectProperty`
`rdfs:domain   :Wine ;`
`rdfs:range      xdsd:integer .`
Then complete the instantation:
`:WegelerRhengauRiesling a :Wine .`
`:isMadeOf :Riesling ;`
`:hasVintageYear 2007 .`		
Properties in general are not functional.
e.g. Wines can be made of multiple grapes


#### OWL - Class Hierarchies, e.g:
`:Wine a owl:Class ;`
`rdfs:subClassOf :AlcoholicBeverage`
`:AlcoholicBeverage a owl:Class ;`
`rdfs:subClassOf :Beverage .`
`:Beverage a owl:Class .`
via inference, Wine is also a subclass of beverage (because it is transitive)


#### OWL - Disjunctiveness, e.g:
`:AlcoholicBeverage owl:disjointWith :MainDish .`
via inference, Wine and Pizza must also be disjoint classes
OWL - Multiple Disjunctiveness, e.g:
`[] a owl:AllDisjointClasses ;`
`owl:members`
`(  :Wine`
`:Beer`
`:SoftDrink`
`:Vegetables`
`:Seafood`
`:Meat  ) .`
	   

#### OWL - Class Equivalence, e.g.
`:AlcoholicBeverage a owl:Class .`
`:Liquor a owl:Class`
`:Wine a owl:Class ;`
`rdfs:subClassOf :AlcoholicBeverage .`
`:AlcoholicBeverage owl:equivalentWith :Liquor .`
via inference, it can be entailed that Wine is also a Liquor


#### Relationships among individuals
`:WegelerRheingauRiesling a :Wine;`
`owl:sameAs  :WRR012345 .`
via inference, WRR012345 is AlcoholicBeverage
`:WRR012346 a :Wine ;`
`owl:differentFrom :WRR012345`

OWL - Multiple different members, e.g.
`[] a owl:AllDifferent ;`
`owl:distinctMembers`
`(:WegerlerRheingauRiesling`
`:Merlot`
`:Chardonnay`
`:Shiraz) .`

OWL - Closed Classes (Nominals)
`:Wine a owl:Class ;`
`:Merlot a :Wine .`
`:Cabernet a :Wine .`
`:RedwinesInStore a owl:Class ;`
`owl:oneOf`
`(:Merlot,`
`:Cabernet) .`
i.e. no other red wine is available in the store


#### OWL - Logical Class Constructors:
logical AND (conjunction):
`owl:intersectionOf`
logical OR (disjunction):
`owl:unionOf`
logical negation (¬):
`owl:complementOf`
Use these to create complex class descriptions from atomic classes
e.g. 1:
`:Wine a owl:Class .`
`:ThingsInStore a owl:Class .`
`:WinesInStore a owl:Class ;`
`owl:intersectionOf (:Wine :ThingsInStore) .`
e.g. 2:
`: Wine a owl:Class ;`
`owl:equivalentClass [`
`owl:unionOf ( :DryWine`
`:MediumWine`
`:SweetWine )`
`] .`
i.e. define a class as the union of other classes
e.g. 3:
`:Wine a owl:Class ;`
`rdfs:SubClassOf [`
`owl:complementOf :Pizza`
`] .`
or can be written as:
`:Wine a owl:Class ;`
`owl:disjointWith :Pizza`


#### OWL - Properties and Property Restrictions
 - Used to describe complex classes via properties

Restrictions on values:
`owl:hasValue`
`owl:allValuesFrom`
`owl:someValuesFrom`

Restrictions on cardinality:
`owl:cardinality`
`owl:maxcardinality`
`owl:mincardinality`

e.g:
`:HaraldsCourses a owl:Class ;`
`rdfs:subClassOf`
`[ a owl:Restriction ;`
`owl:onProperty :isManagedBy ;`
`owl:hasValue :Harald`
`] .`
i.e. Haralds courses must be managed by Harald

e.g (Universal):
`:Wine a owl:Class ;`
`rdfs:subClassOf`
`[ a owl:Restriction ;`
`owl:onProperty :hasProducer ;`
`owl:allValuesFrom :Winemaker`
`] .`
i.e. all wines must be produced by something from class Winemaker

e.g (Existential):
`:WineLover a owl:Class ;`
`rdfs:subClassOf`
`[ a owl:Restriction ;`
`owl:onProperty :loves ;`
`owl:someValuesFrom :Wine`
`] .`
i.e. a WineLover is someone who loves some wine (among other things)

e.g.
`:StringQuartet a owl:Class ;`
`rdfs:subClassOf`
`[ a owl:Restriction ;`
`owl:onProperty :hasMembers ;`
`owl:cardinality 4`
`] .`
A StringQuartet always has exactly 4 members

Qualified Number Restriction, e.g:
`:Examination a owl:Class`
`rdfs:subClassOf [`
`a owl:Restriction ;`
`owl:onProperty :hasExaminer ;`
`owlminQualifiedCardinality "2"^^xsd:nonNegativeInteger;`
`owl:onClass :Professor`
`] .`
An examination has at least two examiners, and they must be Professors


#### OWL - Property Relationships
e.g:
`:hasMother a owl:ObjectProperty ;`
`rdfs:subProperty  Of :hasParent`
	
e.g:
`:hasChild a owl:ObjectProperty ;`
`owl:inverseOf :hasParent;`

Transitive Property:
`owl:TransitiveProperty`
i.e. if isPartOf(a,b) and isPartOf(b,c) then it holds that isPartOf(a,c)
e.g:
`:Region a owl:Class .`
`:England a :Region`
`:isLocatedIn a owl:ObjectProperty ;`
`a owl:TransitiveProperty ;`
`rdfs:domain owl:Thing ;`
`rdfs:range :Region .`
`:Buxton a :Region ;`
`isLocatedIn :Derbyshire .`
`:Derbyshire a :Region ;`
`isLocatedIn :England .`
via inference, Buxton is located in England

Symmetric Property:
`owl:SymmetricProperty`
i.e. if isNeighbourOf(a,b) then it holds that isNeighbourOf(b,a)

Functional Property:
`owl:FunctionalProperty`
i.e. if hasMother(a,b) and hasMother(a,c) then it holds that b=c

Inverse Functional Property:
`owl:InverseFunctionalProperty`
i.e. if isMotherOf(b,a) and isMotherOf(c,a) then it holds that b=c

Asymmetric Property:
`owl:AsymmetricProperty`
i.e. if isLeftOf(a,b), then it not possible that isLeftOf(b,a)

Reflexive Property:
`owl:ReflexiveProperty`
e.g. isRelatedTo(x,x) - x is related to itself

Irreflexive Property:
`owl:IrreflexiveProperty`
i.e. if isParentOf(x,y), then x/=y

Can also define disjunctive properties (like disjunctive classes)
i.e. x and y can never be related by both properties
e.g:
`:hasParent a owl:ObjectProperty`
`owl:propertyDisjointWith :hasChild`
e.g. multiple (all singles pairs are disjoint of each other)
`[] rdf:Type owl:AllDisjointProperties`
`owl:members ( :hasParent :hasChild :hasGrandchild) .`
   
Can also have top and bottom properties
`owl:topObjectProperty`
`owl:bottomObjectProperty`
`owl:topDatatypeProperty`
`owl:bottomDatatypeProperty`



References:
[[Youtube - Semantic Web Technologies (L5)]]
[[W3C - OWL 2 Primer]]
[[Jenkins - ST4SE]]
[[Youtube - Semantic Web Technologies (L5)]]


