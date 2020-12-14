
# Okta APKI Access Management Resource

## Reference

- API Access Management
  + https://www.okta.com/products/api-access-management/
    * OAuth 2.0 API Authorization 
    * Identity-driven Policy Engine 
    * Centralized API Administration, Create, maintain, and audit API access policies.


- https://www.okta.com/identity-101/

- https://developer.okta.com/

- https://www.okta.com/products/customer-identity/b2b-integration/
  + "Easily connect with partners that have their own IDP or access management
    deployment; federate using SAML or OIDC."
  + "Connect your customer's LDAP or Active Directory; synchronize user accounts
    to Universal Directory."
  + "Okta is a customizable identity platform. You can quickly deploy separate
    Okta tenants for each of your customers or partners. "
  + "Connect them to individual applications for each customer, or connect
    everyone to a common application."
  + "Securely segregate each of your own customers with their own Okta tenant."
  + "Defer authentication to AD or LDAP as the source of truth, which allows you to maintain access controls from your local directory rather than store directory credentials in Okta. Delegated authentication is automatic and allows high availability."


- Pricing:
  + https://www.okta.com/pricing/
  + https://www.okta.com/pricing/#api-b2b-integration
    * "Starts at $29,000 annually"
  + https://www.okta.com/pricing/#api-access-management
    * "Starts at $8,000 annually" - User driven flows, priced by MAU
    * "Starts at $5,000 annually" - Machine-to-Machine, priced by tokens


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

  + https://developer.okta.com/docs/guides/protect-your-api/aspnet/before-you-begin/
    * "These steps apply to back-end APIs that are serving single-page apps or
      mobile apps that use Okta to sign users in."

  + https://developer.okta.com/docs/guides/protect-your-api/go/configure-cors/
    * "Configuring Cross-Origin Resource Sharing (CORS) is only required if the
      API is being called from a browser app hosted on a different domain. For
      example, if your single-page JavaScript app is on example.com, but your
      API is hosted on api.example.com, you need to enable CORS."

  + https://developer.okta.com/docs/guides/set-up-event-hook/overview/
    * https://developer.okta.com/docs/concepts/event-hooks/
      * "Event Hooks are outbound calls from Okta, sent when specified events
        occur in your org. They take the form of HTTPS REST calls to a URL you
        specify, encapsulating information about the events in JSON objects in
        the request body. These calls from Okta are meant to be used as triggers
        for process flows within your own software systems."
  
  + https://developer.okta.com/docs/guides/production-deployment/deployment-checklist/


- OAuth 2.0 and OpenID Connect Overview ```*** READ THIS ARTICLE ***```
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


- Authorization Servers
  + https://developer.okta.com/docs/concepts/auth-servers/
    * "You use a Custom Authorization Server to create and apply authorization
      policies to secure your APIs. An access token that is minted by a Custom
      Authorization Server is consumed by your APIs."
    * "Okta allows you to create multiple Custom Authorization Servers within a single Okta org that you can use to protect your own resource servers. Within each authorization server, you can define your own custom OAuth 2.0 scopes, claims, and access policies to support authorization for your APIs.
      * https://developer.okta.com/docs/guides/customize-authz-server/create-scopes/
        * "Scopes specify what access privileges are being requested as part of
          the authorization. For example, the email scope requests access to the
          user's email address. There are certain reserved scopes that are
          created with any Okta authorization server that are listed on the
          OpenID Connect & OAuth 2.0 Scopes section."
        * "If you need scopes in addition to the reserved scopes provided, you
          can create them. Custom scopes can have corresponding claims that tie
          them to some sort of user information."
      * https://developer.okta.com/docs/guides/customize-authz-server/create-claims/
        * "Tokens contain claims that are statements about the subject (for
          example: name, role, or email address)."
      * https://developer.okta.com/docs/guides/customize-authz-server/create-access-policies/
        * "Access policies are containers for rules. Each access policy applies
          to a particular OpenID Connect application, and the rules that it
          contains define different access and refresh token lifetimes depending
          on the nature of the token request."
          
    

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

  + https://developer.okta.com/docs/guides/implement-auth-code/use-flow/
  + https://developer.okta.com/docs/guides/implement-auth-code/exchange-code-token/

  + https://developer.okta.com/docs/guides/implement-oauth-for-okta/request-access-token/

  + https://developer.okta.com/docs/guides/implement-client-creds/overview/
    * "The Client Credentials flow is recommended for server-side (AKA confidential) client applications with no end user, which normally describes machine-to-machine communication. Your application needs to securely store its Client ID and secret and pass those to Okta in exchange for an access token. At a high-level, the flow only has two steps:"
      * "Your application passes its client credentials to your Okta Authorization Server."
      * "If the credentials are accurate, Okta responds with an access token."


  + https://developer.okta.com/docs/guides/validate-access-tokens/
    * "You can use Okta to authenticate your end users and issue them signed
      access and ID tokens, which your application can then use."
    * "It is important that your application only uses the access token to grant
      access, and not the ID token."
    * "After the signed tokens are issued to the end users, they can be passed
      to your application for validation. There are two ways to verify a token:
      locally or remotely with Okta. The token is signed with a JSON Web Key
      (JWK) using the RS256 algorithm. To validate the signature, Okta provides
      your application with a public key that can be used."
        * https://developer.okta.com/docs/guides/validate-access-tokens/go/overview/#access-tokens-vs-id-tokens
        * https://developer.okta.com/docs/guides/validate-access-tokens/go/overview/#what-to-check-when-validating-an-access-token
        * https://developer.okta.com/docs/guides/validate-access-tokens/go/overview/#validating-a-token-remotely-with-okta
    * "The access tokens are in JSON Web Token (JWT) format. They are signed
      using asymmetrical JSON Web Keys (JWK)"
        * [RFC 7517 JSON Web Key (JWK)]((https://tools.ietf.org/html/rfc7517)
        * [RFC 7519 JSON Web Token (JWT)](https://tools.ietf.org/html/rfc7519)


- Scopes
  + https://developer.okta.com/docs/guides/implement-oauth-for-okta/scopes/
  + https://developer.okta.com/docs/guides/implement-oauth-for-okta/define-allowed-scopes/


- Authentication (authn)
  + https://developer.okta.com/product/authentication/
  + https://developer.okta.com/books/api-security/authn/



- Federated Authentication
  + https://developer.okta.com/books/api-security/authn/federated/

