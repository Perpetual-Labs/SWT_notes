# Object-Role Modeling

## Usage
In use by [[ESA]] within [[OSMOSE]]


## Personnel
[[Enrico Franconi]]

## Overview
Fact-based modelling

A conceptual language that has an expressive family of constraints, rich graphical notation and very close to natural language.
In comparison to [[OWL]], it is much easier to learn and use, especially for non-IT people
It is very similar to OWL, but for a few small details, e.g:
 - no nominals
 - no transitivity relations

It is similar to [[UML]]
[[UML]] and ORM have lots of supporting literature


## Reasoning
ORM uses [[OCL]], like [[UML]]
In [[NORMA]], ORM is translated to [[OWL]] (contained in tool)
Can translate anything from ORM to [[OWL]]


## Reasoning Example
 - Citizen has IDCard
 - Visitor has Visa
 - IDCard and Visa are disjoint
 - therefore, inference is that Citizen and Visitor are disjoint



ORM can be used with the [[NORMA]] tool ([[ESA]]'s preference)
- But the NORMA tool is incomplete


References:
[[ESA2019 - Overall System Modelling for Systems Engineering]]
[[OntoCommons]] - Workshops
