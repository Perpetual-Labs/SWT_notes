## MCAD Ontology

Note: not named as such in the paper
Ontology not presented in detail in the paper

#### Overview

MCAD_Entity (e.g. hole, slot)
described by:
MCAD_Component (e.g. axis, depth, etc)

 - Generally:
	 - define features by their function, not their geometry

 - e.g. Hole - have multiple types:
 - Thinning Hole
	 - to reduce mass (volume is interesting bit)
 - Passing Hole
	 - to allow an object to pass through (axis, profile is interesting bit. Depth is derived)
 - Joining Hole
	 - for nuts and bolts etc. (like Passing Hole but axis must be perpendicular to plane)

So define in this way using OWL

When the validity of the feature is altered, the user is notified
but without overconstraining the designer
Can also check for interactions between features


#### MCAD Entities

![[Mandorli - MCAD Entities.jpg]]




#### References
[[Mandorli2020 - From form features to semantic features in existing MCAD. An ontological approach]]