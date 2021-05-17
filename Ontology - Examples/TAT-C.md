https://tatckb.org/

[[Paul Grogan]]

Object schema presented in [[JSON]]
 - tatckb.org/schema
 - So is a list of properties
 - Define an object by its list of attribute-value pairs

Also uses OpenAPI
 - does not quite have user forms
 - but have user interface to inout new data, which is then stored in the [[knowledge base]]
 - e.g. can add a new groundstation (define 'Name', 'Latitude', 'Longitude', 'Altitude')
 - Uses FastAPI ([[Python]], Pydantic). Pulls in from this and then produces HTTP user interfaces.
 - FastAPI converts Python into object schema.
 - Can also enforce rules on data inputs (constraints).

Limitations
 - Inferencing and reasoning not really possible with JSON
 - Object schema: only has 'hasA' or 'isA' relationships.
 - Slightly better than taxonomy
 - But not all the relationships of a full [[ontology]]

