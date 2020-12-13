
# Okta APKI Access Management Resource

## Reference

- https://www.okta.com/products/api-access-management/
  + 2020-12-02 Note: Pricing is mentioned as $2/user/month


- https://developer.okta.com/docs/
  + https://developer.okta.com/docs/reference/

  + Dynamic Client Registration API
    * https://developer.okta.com/docs/reference/api/oauth-clients/
    * "The Dynamic Client Registration API provides operations to register and manage client Applications for use with Okta's OAuth 2.0 and OpenID Connect endpoints. This API largely follows the contract defined in RFC7591: OAuth 2.0 Dynamic Client Registration Protocol and OpenID Connect Dynamic Client Registration 1.0"

- Okta-hosted flows
  + https://developer.okta.com/docs/concepts/okta-hosted-flows/
    * "Okta hosts authentication and identity flows for your applications. This means that your application can let Okta handle signing users in, registering new users, and performing account recovery. The pages hosted by Okta can be customized, and you can bring your own domain."
    * "You can build and self-host these flows in your application if you'd like, but using Okta-hosted flows has some advantages: ..."

- The OpenID Connect redirect flow
  + https://developer.okta.com/docs/concepts/okta-hosted-flows/#the-openid-connect-redirect-flow

- Recommended flow by application type
  + https://developer.okta.com/docs/concepts/oauth-openid/#recommended-flow-by-application-type


- https://developer.okta.com/product/
  + "Build your app. We’ll handle the Authorization."

- API Security
  + https://developer.okta.com/books/api-security/


- OAuth 2.0 and OpenID Connect Overview
  + https://developer.okta.com/docs/concepts/oauth-openid/
    * "To decide which authentication flow is best for you based on the type of
      application that you are building, you first need to understand OAuth 2.0
      and OpenID Connect and how you can implement these two flows using Okta."


- OpenID Connect & OAuth 2.0 API ```***  READ THIS ARTICLE ***```
  + https://developer.okta.com/docs/reference/api/oidc/
    * Okta is a standards-compliant OAuth 2.0 authorization server and a certified OpenID Connect provider 
    * OpenID Connect extends OAuth 2.0. The OAuth 2.0 protocol provides API security via scoped access tokens, and OpenID Connect provides user authentication and single sign-on (SSO) functionality.


- Managing API Credentials
  + https://developer.okta.com/books/api-security/api-keys/

- Authorization (authz)
  + https://developer.okta.com/product/authorization/
  + https://developer.okta.com/books/api-security/authz/

  + https://developer.okta.com/docs/guides/implement-auth-code-pkce/overview/
    * "If you are building a native application, then the Authorization Code
      flow with a Proof Key for Code Exchange (PKCE) is the recommended method
      for controlling the access between your application and a resource
        server."

  + https://developer.okta.com/docs/guides/implement-auth-code/overview/
    * "If you are building a server-side (or web) application that is capable of securely storing secrets, then the authorization code flow is the recommended method for controlling access to it."

  + https://developer.okta.com/docs/guides/implement-client-creds/overview/
    * "The Client Credentials flow is recommended for server-side (AKA confidential) client applications with no end user, which normally describes machine-to-machine communication. Your application needs to securely store its Client ID and secret and pass those to Okta in exchange for an access token. At a high-level, the flow only has two steps:"
      * "Your application passes its client credentials to your Okta Authorization Server."
      * "If the credentials are accurate, Okta responds with an access token."


- Authentication (authn)
  + https://developer.okta.com/product/authentication/
  + https://developer.okta.com/books/api-security/authn/

- https://developer.okta.com/books/api-security/authn/federated/

