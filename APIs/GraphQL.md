
# GraphQL API Resources


## Github Resources
- https://github.com/ibm/openapi-to-graphql
  + "Translate APIs described by OpenAPI Specifications (OAS) or Swagger into GraphQL."
  + https://developer.ibm.com/open/projects/openapi-to-graphql/
  + Papers
    * [Generating GraphQL-Wrappers for REST(-like) APIs](https://arxiv.org/abs/1809.08319)
      * "GraphQL is a query language and thereupon-based paradigm for implementing web Application Programming Interfaces (APIs) for client-server interactions. Using GraphQL, clients define precise, nested data-requirements in typed queries, which are resolved by servers against (possibly multiple) backend systems, like databases, object storages, or other APIs. Clients receive only the data they care about, in a single request. However, providers of existing REST(-like) APIs need to implement additional GraphQL interfaces to enable these advantages. We here assess the feasibility of automatically generating GraphQL wrappers for existing REST(-like) APIs. A wrapper, upon receiving GraphQL queries, translates them to requests against the target API. We discuss the challenges for creating such wrappers, including dealing with data sanitation, authentication, or handling nested queries. We furthermore present a prototypical implementation of OASGraph. OASGraph takes as input an OpenAPI Specification (OAS) describing an existing REST(-like) web API and generates a GraphQL wrapper for it. We evaluate OASGraph by running it, as well as an existing open source alternative, against 959 publicly available OAS. This experiment shows that OASGraph outperforms the existing alternative and is able to create a GraphQL wrapper for 89.5% of the APIs -- however, with limitations in many cases. A subsequent analysis of errors and warnings produced by OASGraph shows that missing or ambiguous information in the assessed OAS hinders creating complete wrappers. Finally, we present a use case of the IBM Watson Language Translator API that shows that small changes to an OAS allow OASGraph to generate more idiomatic and more expressive GraphQL wrappers."


