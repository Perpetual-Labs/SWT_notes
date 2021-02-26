
# Linked Data
Large non-[[Semantics|semantic]] datasets results in a high level of human effort for finding, retrieving and exploiting information.
Such issues dramatically reduce the value of the information discovered as well as the ability to automate the consumption of such data.
The aim of the Linked Data approach is to solve these issues.

For the machine interpretation of semantic content to become possible, there are two prerequisites:
- **Every [[Resources|resource]] should be uniquely identified**. The [[Semantic Web]] solves such issues by adopting unique identifiers for concepts and the relationships between them. These identifiers, called [[URI]]
- **There must be a unified system for conveying and interpreting meaning** that all automated search agents, data storage applications and analysers should use. This is achieved by making use of formal [[Ontology|ontologies]] – hierarchical structures of concepts – to classify individual concepts, thus making it possible to infer new information based on an individual’s classification and relationship to other concepts. 

The necessary machine-processable information can be embedded in the dataset through the use of special meta-descriptors (meta-tagging). Within these meta tags, the resources (the pieces of useful information) can be uniquely identified (using URIs) and the semantic relationships between resources can be formally described in terms of properties and values using a language that is machine interpretable. The concrete implementations of these conventions can be achieved using a appropriate data-model (such as [[RDF]]) and semantic schemata and languages (such as [[RDFS]] and [[OWL]].


For further info:
[[Youtube - Semantic Web Technologies (L6)]]

References:
[[Blog2020 - Introduction to the Semantic Web]]
