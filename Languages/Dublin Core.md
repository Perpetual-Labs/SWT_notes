An example of a shared vocabulary that is readily available for reuse is The Dublin Core, which is a set of elements ([[Properties]]) for describing documents (and hence, for recording metadata). 

 - One of the most popular vocabularies for use with [[RDF]]
 - Linked to the [[Linked Data]] movement


Detail:

The goal of Dublin Core is to provide a minimal set of descriptive elements that facilitate the description and the automated indexing of document-like networked objects, in a manner similar to a library card catalogue. 
Dublin Core elements have become widely used in documenting Internet resources (the Dublin Core `creator` element was used in the earlier examples). The current elements of Dublin Core contain definitions for properties such as `title` (a name given to a resource), `creator` (an entity primarily responsible for creating the content of the resource), `date` (a date associated with an event in the life-cycle of the resource) and `type` (the nature or genre of the content of the resource).

Example:

The following example uses Dublin Core by itself to describe an audio recording of a guide to growing rose bushes:

	<rdf:RDF
			xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"
			xmlns:dc="http://purl.org/dc/elements/1.1/">

		<rdf:Description rdf:about="http://media.example.com/audio/guide.ra">
			<dc:creator>Mr. Dan D. Lion</dc:creator>
			<dc:title>A Guide to Growing Roses</dc:title>
			<dc:description>Describes planting and nurturing rose bushes.
			</dc:description>
			<dc:date>2001-01-20</dc:date>
		</rdf:Description>
	</rdf:RDF>