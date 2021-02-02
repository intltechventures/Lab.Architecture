
# Dell Boomi Resources


## References

- https://boomi.com/

- https://help.boomi.com/bundle/release-notes/

- https://community.boomi.com/
  + https://community.boomi.com/s/forums#sort=relevancy


## Limitations

- As of 2021-02-01, it appears that Dell Boomi does not yet support OpenAPI Specification 3.x
  + https://community.boomi.com/s/question/0D51W00007lfZqsSAE/currently-generated-swagger-specification-files-are-based-on-swagger-v20-and-swagger-specification-files-imported-into-api-proxy-components-must-be-v20compliant-when-is-boomi-going-to-implement-current-openapi-specification-302
  + https://help.boomi.com/bundle/integration/page/c-atm-Swagger_specification_for_an_API_component.html
    * "The current version of Swagger is 2.0. Generated Swagger specification files for API Service components are based
      on Swagger v2.0. Swagger specification files imported into API Proxy components must be v2.0-compliant and in JSON
      or YAML format."
  + https://dzone.com/articles/build-an-api-using-aws-api-gateway-and-dell-boomi
    * "We would use swagger 2.0 instead of the newer version of OAS 3.0 because this is recognized by both AWS and Dell
      Boomi."

- https://help.boomi.com/bundle/api_management/page/c-atm-API_design.html
  + As of 2021-02-01, it appears that there are severly limited API design options - and WSDL/SOAP seem to be the
    predominate option. No mention of OpenAPI Specification (OAS) support.
  + However, Swagger and REST are mentioned here:
    * https://help.boomi.com/bundle/api_management/page/int-API_Service_components.html


