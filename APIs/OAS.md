
# OpenAPI Specification (OAS) Resources

## References
- https://en.wikipedia.org/wiki/OpenAPI_Specification

- https://www.openapis.org/
  + http://spec.openapis.org/oas/v3.0.2

- https://github.com/OAI
- https://github.com/OAI/OpenAPI-Specification
  + https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.2.md


## 3.0 Specification Implementations
- https://github.com/OAI/OpenAPI-Specification/blob/master/IMPLEMENTATIONS.md#implementations


## Third-Party Resources
- https://openapi.tools/

- https://openapi-generator.tech/
  + Generate clients, servers, and documentation from OpenAPI 2.0/3.x documents
  + https://openapi-generator.tech/docs/generators
  + https://github.com/OpenAPITools/openapi-generator

- https://apis.guru/openapi-directory/

- http://speccy.io/
  + A handy toolkit for OpenAPI, with a linter to enforce quality rules, documentation rendering, and resolution.
  + https://github.com/wework/speccy
  + https://www.npmjs.com/package/speccy

- https://stoplight.io/spectral
  + https://github.com/openapi-contrib/style-guides
  + https://stoplight.io/p/docs/gh/stoplightio/spectral/docs/getting-started/rulesets.md
  + https://stoplight.io/p/docs/gh/stoplightio/spectral/docs/guides/workflows.md#git-hooks
    * https://github.com/typicode/husky
      * https://github.com/typicode/husky#ci-servers
  + https://git-scm.com/docs/githooks

- https://www.apimatic.io/transformer/
  + "Transform API specifications to formats of your choice"
  + https://www.apimatic.io/transformer/#supported-formats
  + https://github.com/LucyBot-Inc/api-spec-converter

- https://swagger.io/tools/swagger-codegen/
  + "Swagger Codegen can simplify your build process by generating server stubs and client SDKs for any API, defined with the OpenAPI (formerly known as Swagger) specification, so your team can focus better on your API’s implementation and adoption."


## Github Resources

- https://github.com/api-specification-toolbox

- https://github.com/deepmap/oapi-codegen
  + Generate Go client and server boilerplate from OpenAPI 3 specifications 

- https://github.com/APIs-guru/awesome-openapi3
  + https://apis.guru/awesome-openapi3/

- https://github.com/openapitools/openapi-generator/
  + "OpenAPI Generator allows generation of API client libraries (SDK generation), server stubs, documentation and configuration automatically given an OpenAPI Spec (v2, v3)"
  + https://openapi-generator.tech/
    * https://openapi-generator.tech/docs/usage
  + https://github.com/OpenAPITools/openapi-style-validator
    * "A customizable style validator to make sure your OpenApi spec follows your organization's standards."

- https://github.com/LucyBot-Inc/api-spec-converter

- https://github.com/readmeio/oas
  + https://openap.is/
    * "A language-agnostic tool for documenting your API right from your code, generating an OpenAPI Spec, and sharing it via a URL."

- https://github.com/APIs-guru/openapi-directory/
  + "Wikipedia for Web APIs. Directory of REST API definitions in OpenAPI 2.0/3.0 format"
  + https://apis.guru/openapi-directory/

- https://github.com/wework/speccy
  + "Speccy aims to become the rubocop or eslint of OpenAPI."
  + http://speccy.io/
  + https://apisyouwonthate.com/blog/govern-your-apis-with-speccy
    * "Update (2019-10-04): When I left WeWork I left Speccy with a few colleagues, who have thankfully done a lot of maintainance work. If you like the idea of Speccy but want more power, use Spectral by Stoplight. It has a bunch of developers and community contributors regularly adding amazing features, and does everything Speccy used to do and loads more. See how you can use this, and other tools, to make automated enforceable style guides!"

- https://github.com/stoplightio/spectral
  + "A flexible JSON/YAML linter for creating automated style guides, with baked in support for OpenAPI v2 & v3."
  + https://stoplight.io/spectral
    * https://github.com/openapi-contrib/style-guides

- https://github.com/Mermade/oas-kit/
  + "Convert Swagger 2.0 definitions to OpenAPI 3.0 and resolve/validate/lint"
  + https://mermade.org.uk/openapi-converter

- https://github.com/openapi-contrib/style-guides
  + A shared and somewhat opinionated style guide for everyone to enjoy. 
  + https://github.com/openapi-contrib/style-guides/blob/master/openapi.yml

- https://github.com/Redocly/redoc
  + https://redocly.github.io/redoc/
  + Example:
    * https://github.com/Redocly/create-openapi-repo


- https://github.com/hakopako/openapi-cli-tool
  + "OpenAPI (Swagger 3.x) CLI Tool. Supports multiple file extensions. Can list up defined API paths and bundle multi-file into one."
  + https://pypi.org/project/openapi-cli-tool/
    * "OAS interactive scaffolding."


- https://github.com/ibm/openapi-to-graphql
  + https://developer.ibm.com/open/projects/openapi-to-graphql/
  + https://www.npmjs.com/package/openapi-to-graphql-cli
    * "Command line interface (CLI) for turning APIs described by OpenAPI Specification (OAS) into GraphQL interfaces."
    * https://arxiv.org/abs/1809.08319
      * "Generating GraphQL-Wrappers for REST(-like) APIs"
        * "Our research paper, "Generating GraphQL-Wrappers for REST(-like) APIs", can be found here. The paper describes the challenges of building OpenAPI-to-GraphQL and an experiment in which we evaluated OpenAPI-to-GraphQL against 959 publicly available OAS, provided by APIs.guru, and successfully created GraphQL interfaces for 89.5% of them."



## IDE Tooling

### Visual Studio Code
- https://marketplace.visualstudio.com/items?itemName=42Crunch.vscode-openapi

- https://marketplace.visualstudio.com/items?itemName=mermade.openapi-lint

- https://marketplace.visualstudio.com/items?itemName=zoellner.openapi-preview

- https://marketplace.visualstudio.com/items?itemName=philosowaffle.openapi-designer

- https://www.eclipse.org/codewind/open-api-tools-for-vscode.html


### Eclipse
- https://marketplace.eclipse.org/content/openapi-studio-rich-oas3-editor



## Interesting News Items

### 2021 


### 2020
- 2020-12-08 MicroProfile OpenAPI Specification, Version: 2.0, Status: Final, Release: December 08, 2020
  + https://download.eclipse.org/microprofile/microprofile-open-api-2.0/microprofile-openapi-spec-2.0.html


- 2020-02-02 OpenAPI v3.1 and JSON Schema 2019-09
  + https://apisyouwonthate.com/blog/openapi-v31-and-json-schema-2019-09
    * "The Schema Object allows the definition of input and output data types. These types can be objects, but also primitives and arrays. This object is a superset of the JSON Schema Draft 2019-09 specification."
      * https://json-schema.org/draft/2019-09/json-schema-core.html
      * https://json-schema.org/draft/2019-09/json-schema-validation.html
    * "If a keyword exists in JSON Schema Draft 2019-09 (Core or Validation), then it's good to use in OpenAPI v3.1."


