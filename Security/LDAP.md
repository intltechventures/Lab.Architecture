
# Lightweight Directory Access Protocol (LDAP) Resources


## References
- https://en.wikipedia.org/wiki/Lightweight_Directory_Access_Protocol
  + "directory services may provide any organized set of records, often with a
    hierarchical structure"
  + "A common use of LDAP is to provide a central place to store usernames and
    passwords."

- [RFC 4511 Lightweight Directory Access Protocol (LDAP): The Protocol](https://tools.ietf.org/html/rfc4511)

- [RFC 4533 The Lightweight Directory Access Protocol (LDAP) Content Synchronization Operation](https://tools.ietf.org/html/rfc4533)


- https://en.wikipedia.org/wiki/Directory_service
  + "...a directory service or name service maps the names of network resources to their respective network addresses. It is a shared information infrastructure for locating, managing, administering and organizing everyday items and network resources, which can include volumes, folders, files, printers, users, groups, devices, telephone numbers and other objects. "
  + "A directory service defines a namespace for the network."
  + "The namespace is used to assign a name (unique identifier) to each of the objects. Directories typically have a set of rules determining how network resources are named and identified, which usually includes a requirement that the identifiers be unique and unambiguous."
  + "The Lightweight Directory Access Protocol (LDAP) is based on the X.500
    directory-information services, using the TCP/IP stack and an X.500
    Directory Access Protocol (DAP) string-encoding scheme on the Internet."
  + "LDAP is based on a simpler subset of the standards contained within the
    X.500 standard. Because of this relationship, LDAP is sometimes called
    X.500-lite."
  + Operations:
    * Add
    * Bind (authenticate)
    * Delete 
    * Search and Compare 
    * Modify 
    * Modify Distinguished Name (DN) 
    * Extend operations
      * StartTLS 
    * Abandon 
    * Unbind (close connection, not the inverse of Bind)
  + Directory Structure:
    * An entry, with a set of attriutes 
    * An attribute has a name and one or more values
    * Each entry has a unique identifier, its Distinguished Name (DN)
  + "LDAP rarely defines any ordering: The server may return the values of an
    attribute, the attributes in an entry, and the entries found by a search
    operation in any order. "

## OpenLDAP.org
- https://www.openldap.org/

- https://www.openldap.org/doc/

- https://www.openldap.org/software/man.cgi

- https://en.wikipedia.org/wiki/OpenLDAP
  + "Derived from the original University of Michigan LDAP implementation (like
    Netscape, Red Hat, Fedora and Sun JSDS implementations), it supports all
    computer architectures (including Unix and Unix derivatives, Linux, Windows,
    z/OS and a number of embedded-realtime systems)."
  + "an open, vendor-neutral, industry standard application protocol for
    accessing and maintaining distributed directory information services over an
    Internet Protocol (IP) network."
  + OpenLDAP has three main components:
    * slapd – stand-alone LDAP daemon and associated modules and tools
      * "The slapd server can use arbitrarily many backends at once, and can
        have arbitrarily many instances of each backend (i.e., arbitrarily many
        databases) active at once. "
    * libraries implementing the LDAP protocol and ASN.1 Basic Encoding Rules (BER)
    * client software: ldapsearch, ldapadd, ldapdelete, and others
  + "Ordinarily an LDAP request is received by the frontend, decoded, and then
    passed to a backend for processing. When the backend completes a request, it
    returns a result to the frontend, which then sends the result to the LDAP
    client. An overlay is a piece of code that can be inserted between the
    frontend and the backend. It is thus able to intercept requests and trigger
    other actions on them before the backend receives them, and it can also
    likewise act on the backend's results before they reach the frontend.
    Overlays have complete access to the slapd internal APIs, and so can invoke
    anything the frontend or other backends could perform. Multiple overlays can
    be used at once, forming a stack of modules between the frontend and the
    backend. "
  + "Overlays provide a simple means to augment the functionality of a database
    without requiring that an entirely new backend be written, and allow new
    functionalities to be added in compact, easily debuggable and maintainable
    modules. Since the introduction of the overlay feature in OpenLDAP 2.2 many
    new overlays have been contributed from the OpenLDAP community. "
  + "Currently there are 21 overlays in the core OpenLDAP distribution, with
    another 15 overlays in the user-contributed code section, and more awaiting
    approval for inclusion. "
  + "OpenLDAP supports replication using Content Synchronization as specified in
    RFC 4533"



