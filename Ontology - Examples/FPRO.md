## Feature-based Product Ontology (FPRO)

#### Overview

Based on [[LUPO]]
Built in [[Protege]] using [[OWL]]
Ontology for [[Additive Manufacturing]]
Similar to [[Belkadi Framework]], more detail on features, less on processes


#### Structure

 - Captures PFeatures and IFeatures
	 - PFeatures are features of a physical object
		 - PFeatures can be categorised by 'Form' (e.g. 'BendPFeature', 'HolePFeature')
		 - or by 'ManufacturingProcess' (e.g. 'AdditivePFeature')
	 - IFeatures are the information that describe PFeature

 - This is done because:
	 - Geometric formalisms do not allow for the explicit embedding of design intents into product models (e.g. functional or manufacturing intent)
	 - Aim is understand 'features' ontologically - independent of CAx implementation

 - Example Rules:
	 - material feature cannot be feature of immaterial object


#### PFeatures Taxonomy

![[FPRO - PFeature Taxonomy.jpg]]


#### Types

 - Interesting use of class 'Type' - e.g. material, process, etc.
	 - i.e. Material is nonPhysical; Material physicallyRealizedBy PhysicalObject


#### Interesting Notes

 - The authors reference other issues with the 'isAbout' some real entity
	 - i.e. when the 'system' in SE doesn't exist yet

 - Top-level distinction between PhysicalArtifact and Person


#### References
[[Sanfilippo2018 - Feature-based product modelling. An ontological approach]]
[[Sanfilippo2019 - Ontology-based knowledge representation for additive manufacturing]]
