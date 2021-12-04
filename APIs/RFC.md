
# RFC Resources, re: APIs



- [RFT 6750 The OAuth 2.0 Authorization Framework: Bearer Token Usage](https://datatracker.ietf.org/doc/html/rfc6750.html)

- [RFC 7525 Recommendations for Secure Use of Transport Layer Security (TLS) and Datagram Transport Layer Security (DTLS)](https://datatracker.ietf.org/doc/html/rfc7525)

- [RFC 7636 Proof Key for Code Exchange by OAuth Public Clients](https://tools.ietf.org/html/rfc7636)

- [RFC 8996 Deprecating TLS 1.0 and TLS 1.1](https://datatracker.ietf.org/doc/html/rfc8996)
  + "Implementations MUST NOT negotiate SSL version 2"
  + "Implementations MUST NOT negotiate SSL version 3"
  + "Implementations SHOULD NOT negotiate TLS version 1.0 [RFC2246]"
  + "Implementations SHOULD NOT negotiate TLS version 1.1 [RFC4346]"
  + "Implementations MUST support TLS 1.2 [RFC5246] and MUST prefer to negotiate TLS version 1.2 over earlier versions of TLS"
  + "HTTP client and server implementations MUST support the HTTP Strict Transport Security (HSTS) header [RFC6797], in order to allow Web servers to advertise that they are willing to accept TLS-only clients"
  + "Web servers SHOULD use HSTS to indicate that they are willing to accept TLS-only clients, unless they are deployed in such a way that using HSTS would in fact weaken overall security (e.g., it can be problematic to use HSTS with self-signed certificates, as described in Section 11.3 of [RFC6797])"



