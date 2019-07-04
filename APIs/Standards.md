
# API Standards

## HTTP Response Codes
- [RFC-7231:  Hypertext Transfer Protocol (HTTP/1.1): Semantics and Content, 6.  Response Status Codes](https://tools.ietf.org/html/rfc7231#section-6)

    
   | Code | Reason-Phrase                 | Defined in...            |
   |------|-------------------------------|--------------------------|
   | 100  | Continue                      | Section 6.2.1            |
   | 101  | Switching Protocols           | Section 6.2.2            |
   | 200  | OK                            | Section 6.3.1            |
   | 201  | Created                       | Section 6.3.2            |
   | 202  | Accepted                      | Section 6.3.3            |
   | 203  | Non-Authoritative Information | Section 6.3.4            |
   | 204  | No Content                    | Section 6.3.5            |
   | 205  | Reset Content                 | Section 6.3.6            |
   | 206  | Partial Content               | Section 4.1 of [RFC7233] |
   | 300  | Multiple Choices              | Section 6.4.1            |
   | 301  | Moved Permanently             | Section 6.4.2            |
   | 302  | Found                         | Section 6.4.3            |
   | 303  | See Other                     | Section 6.4.4            |
   | 304  | Not Modified                  | Section 4.1 of [RFC7232] |
   | 305  | Use Proxy                     | Section 6.4.5            |
   | 307  | Temporary Redirect            | Section 6.4.7            |
   | 400  | Bad Request                   | Section 6.5.1            |
   | 401  | Unauthorized                  | Section 3.1 of [RFC7235] |
   | 402  | Payment Required              | Section 6.5.2            |
   | 403  | Forbidden                     | Section 6.5.3            |
   | 404  | Not Found                     | Section 6.5.4            |
   | 405  | Method Not Allowed            | Section 6.5.5            |
   | 406  | Not Acceptable                | Section 6.5.6            |
   | 407  | Proxy Authentication Required | Section 3.2 of [RFC7235] |
   | 408  | Request Timeout               | Section 6.5.7            |
   | 409  | Conflict                      | Section 6.5.8            |
   | 410  | Gone                          | Section 6.5.9            |
   | 411  | Length Required               | Section 6.5.10           |
   | 412  | Precondition Failed           | Section 4.2 of [RFC7232] |
   | 413  | Payload Too Large             | Section 6.5.11           |
   | 414  | URI Too Long                  | Section 6.5.12           |
   | 415  | Unsupported Media Type        | Section 6.5.13           |
   | 416  | Range Not Satisfiable         | Section 4.4 of [RFC7233] |
   | 417  | Expectation Failed            | Section 6.5.14           |
   | 426  | Upgrade Required              | Section 6.5.15           |
   | 500  | Internal Server Error         | Section 6.6.1            |
   | 501  | Not Implemented               | Section 6.6.2            |
   | 502  | Bad Gateway                   | Section 6.6.3            |
   | 503  | Service Unavailable           | Section 6.6.4            |
   | 504  | Gateway Timeout               | Section 6.6.5            |
   | 505  | HTTP Version Not Supported    | Section 6.6.6            |



## OpenAPI Specification (OAS)
- https://openapis.org

- https://github.com/oai

- https://github.com/OAI/OpenAPI-Style-Guide
  + "On Nov. 5, 2015, SmartBear in conjunction with 3Scale, Apigee, Capital One, Google, IBM, Intuit, Microsoft, PayPal, and Restlet announced the formation of the OpenAPI Initiative, an open source project under the Linux Foundation. As part of the formation of the OAI, SmartBear donated the Swagger specification to the Linux Foundation, meaning that the OpenAPI Specification is semantically identical to the specification formerly known as the Swagger 2.0 specification. It is widely recognized as the most popular open source framework for defining and creating RESTful APIs, and today tens of thousands of developers are building thousands of open source repos of tools leveraging the OpenAPI Specification. In 2010, the Swagger specification was created by Wordnik, who published it under an open source license one year later. In March of 2015, SmartBear acquired Wordnik's interests in the Swagger projects from its parent company, Reverb Technologies."

- https://github.com/OAI/OpenAPI-Specification
  + https://github.com/OAI/OpenAPI-Specification/tree/master/versions
    * https://github.com/OAI/OpenAPI-Specification/blob/master/versions/2.0.md
    * https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.2.md


## Swagger
- https://swagger.io/
  + https://swagger.io/resources/open-api/
  + https://swagger.io/solutions/getting-started-with-oas/
  + https://swagger.io/docs/open-source-tools/swagger-editor/
  + https://swagger.io/docs/specification/about/
    * https://swagger.io/specification/v2/
    * https://swagger.io/specification/
  + https://swagger.io/tools/open-source/open-source-integrations/   

- https://en.wikipedia.org/wiki/Swagger_(software)
  + "In November 2015, SmartBear Software, the company that maintained Swagger, announced that it was helping create a new organization, under the sponsorship of the Linux Foundation, called the Open API Initiative. A variety of companies, including Google, IBM and Microsoft are founding members."
  + On 1 January 2016, the Swagger specification was renamed to OpenAPI Specification, and was moved to a new repository in [GitHub](https://github.com/OAI/OpenAPI-Specification)
