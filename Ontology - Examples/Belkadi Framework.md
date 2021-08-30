## Belkadi Framework

NOTE: not named in the Belkadi paper
An [[ontology]] for [[Additive Manufacturing]]
Similar to [[FPRO]]
Less detail on features, more on processes

#### Overview

[[Ontology]] for [[Additive Manufacturing]]

 - Requires a combination of [[BPMN]] and [[UML]]
	 - Uses BPMN for AM process definition
	 - Uses UML to define subprocesses
	 - BPMN describes activities and decisions well, but not the participants (i.e. the objects) - so need UML too

 - Previous projects stored in the knowledge base
	 - and referred to each time a new project is started
	 - e.g. Activity: tesselateModel (hasInput geometricProductModel, hasOuput tesselatedModel) - common to all projects with CAD


#### Physical Objects

![[Belkadi - Physical Objects.jpg]]


#### Business Roles

![[Belkadi - Business Roles.jpg]]


#### Technical Descriptions

![[Belkadi - Technical Descriptions.jpg]]

This is like a limited version of [[IAO]]

#### AM Parameters

![[Belkadi - AM Parameters.jpg]]

![[Belkadi - Parameter Dependencies.jpg]]


#### AM Processes

![[Belkadi - AM Processes.jpg]]

Model for process representation distinguishes between material removal, material conservation, joining. Very similar to [[FPRO]]

![[Belkadi - AM Process Relationships.jpg]]

Good process template: input, output, parameter, mechanism, control

#### AM Example

Example provided for the BPMN Process Diagram: "ManufactureJob" - which comprises three activities

![[Belkadi - BPMN Process and Activities.jpg]]

![[Belkadi - Activity 1 Instance.jpg]]

![[Belkadi - Activity 2 Instance.jpg]]

![[Belkadi - Activity 3 Instance.jpg]]



#### References:
[[Belkadi2020 - A Product-Process Model for Decision-Aid Perspective in Additive Manufacturing Field]]