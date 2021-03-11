## Overall System Modelling for Systems Engineering

## Goal
To develop the [[Space Systems Ontology]] - uses [[OWL]]
Under development by [[MB4SE]] Working Group
 - details of the [[Space Systems Ontology]] provided at link.

## Problem Statement
 - Issues associated with [[Standard - ECSS-E-TM-10-23A]]
 - lack of semantic compatibility between suppliers and customers
 - Proven insufficient for one partner to supply a specific view of the data
 - Proven insufficient to apply an excahnge standard that one partner promotes
 - So want to develop OSMoSE - a global space system ontology

## Solution
Address interoperability at [[Semantics|semantic]] level:
Information modelling at system specification level
i.e. Build a global conceptual data model for the Space System - the [[Space System Ontology]]

Space System Ontology governed by two groups:
 - Management Steering Group ([[MB4SE]] Advisory Group)
 - Design Authority Group (OSMOSE WG)

## Tools and Languages
These UoDs will be conceptualised using [[ORM]] and [[NORMA]] Pro.
Then use translation tools to automatically generate e.g. [[UML]], [[Ecore]], [[XML]]

## OSMOSE Outputs
The ORM model of the SSO

		
## [[Ontology]] Advice - Bolzano
 - "The ontologist needs a tool that checks continuously the ontology at each step of its decvelopment and ensures its overall consistency and quality"
 - "The advice is do not use [[OWL]] as a user, but let tools use OWL for you"
 - "Therefore [[ORM]] is preferred, as it is expressive graphical and concise"	
		

## Detailed Plan
From [[ESA2020 - OSMOSE Executive Summary Report]]
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


References:
[[ESA2019 - Overall System Modelling for Systems Engineering]]
[[ESA2020 - OSMOSE Executive Summary Report]]
[[Standard - ECSS-E-TM-10-23A]]
[[Standard - ECSS-E-ST-10C - System engineering general requirements]]
