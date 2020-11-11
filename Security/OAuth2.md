
# OAuth 2 Resources

## References


- https://tools.ietf.org/html/draft-ietf-oauth-security-topics-16


### OAuth 2.1

- https://tools.ietf.org/html/draft-ietf-oauth-v2-1-00  

- https://oauth.net/2.1/
  + The major differences from OAuth 2.0 are listed below.
    * PKCE is required for all OAuth clients using the authorization code flow
    * Redirect URIs must be compared using exact string matching
    * The Implicit grant (response_type=token) is omitted from this specification
    * The Resource Owner Password Credentials grant is omitted from this specification
    * Bearer token usage omits the use of bearer tokens in the query string of URIs
    * Refresh tokens for public clients must either be sender-constrained or one-time use


## Github Resources

- https://www.ory.sh/hydra/
  + https://github.com/ory
  + https://github.com/ory/hydra
    * "OAuth2 Server and OpenID Certified™ OpenID Connect Provider written in Go -
    cloud native, security-first, open source API security for your
    infrastructure. SDKs for any language. Compatible with MITREid."
  + https://www.ory.sh/hydra/docs/
    * "ORY Hydra is a Certified OpenID Provider Server and implements all the
      requirements stated by the OpenID Foundation. In particular, it correctly
      implements the various OAuth 2.0 and OpenID Connect flows specified by the
      IETF and OpenID Foundation."
    * "ORY Hydra offers a safe storage for cryptographic keys (used for example
      to sign JSON Web Tokens) and can manage OAuth 2.0 Clients."
    * "ORY Hydra does not manage user accounts, i.e. user registration, password
      reset, user login, sending confirmation emails, etc. In Hydra's
      architecture, the Identity Provider is responsible for this."
    * "ORY Hydra doesn't support the OAuth 2.0 Resource Owner Password
      Credentials flow because it is legacy, discouraged, and insecure."
  + https://hub.docker.com/r/oryd/hydra/


- https://github.com/ory/fosite 
  + Extensible security first OAuth 2.0 and OpenID Connect SDK for Go. 


## Open Source Solutions 

- https://www.keycloak.org/
  + https://www.keycloak.org/documentation
    * https://www.keycloak.org/docs/latest/getting_started/index.html
    * https://www.keycloak.org/docs/latest/server_admin/
      * "OpenID Connect support."
      * "OAuth 2.0 support."
      * "SAML support."
      * "Identity Brokering - Authenticate with external OpenID Connect or SAML
        Identity Providers."
      * "Social Login - Enable login with Google, GitHub, Facebook, Twitter, and
        other social networks."
      * "User Federation - Sync users from LDAP and Active Directory servers."
  + https://www.keycloak.org/downloads


## Commercial Solutions




## Articles

### 2020 

- 2020-04-15 [What's new in OAuth 2.1?](https://fusionauth.io/blog/2020/04/15/whats-new-in-oauth-2-1/)

- 2020-04-09 YouTube OktaDev Channel, [What's New With OAuth and OIDC?]([https://www.youtube.com/watch?v=g_aVPdwBTfw)



### 2019 

- 2019-12-13 [OAuth 2.1: How Many RFCs Does it Take to Change a Lightbulb?](https://developer.okta.com/blog/2019/12/13/oauth-2-1-how-many-rfcs)

- 2019-12-12 [It's Time for OAuth 2.1](https://aaronparecki.com/2019/12/12/21/its-time-for-oauth-2-dot-1)




