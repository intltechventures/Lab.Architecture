
# DMZ Security Resources

A Security & Network Architecture question recently arose during a client
consulting engagment - and there appears to be dissenting opinions between
different architects on whether a DMZ is needed - or whether it is a relic of
out-dated thinking. 

This document is intended to as my mechanism to collect and organize information
related to various approaches, arguments, rationale - for/against a DMZ in a
modern network architecture (and with a particular interest in hybrid
infrastructure models).

## References

- https://en.wikipedia.org/wiki/DMZ_(computing)
  + For security, compliance with legal standards such as HIPAA, and monitoring reasons, in a business environment, some enterprises install a proxy server within the DMZ. This has the following benefits:
    * Obliges internal users (usually employees) to use the proxy server for Internet access.
    * Reduced Internet access bandwidth requirements since some web content may be cached by the proxy server.
    * Simplifies recording and monitoring of user activities.
    * Centralized web content filtering.

### Microsoft Azure 
- https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/decision-guides/software-defined-network/cloud-dmz
  + "The Cloud DMZ network architecture allows limited access between your
    on-premises and cloud-based networks, using a virtual private network (VPN)
    to connect the networks. Although a DMZ model is commonly used when you want
    to secure external access to a network, the Cloud DMZ architecture discussed
    here is intended specifically to secure access to the on-premises network
    from cloud-based resources and vice versa."

- https://docs.microsoft.com/en-us/azure/architecture/reference-architectures/dmz/secure-vnet-dmz
  + "This reference architecture shows a secure hybrid network that extends an
    on-premises network to Azure. The architecture implements a DMZ, also called
    a perimeter network, between the on-premises network and an Azure virtual
    network. All inbound and outbound traffic passes through Azure Firewall."



## General Background Reading

- https://www.enterprisecloudcustomercouncil.com/documents 
- [Framework for DMZ Architectures for Hybrid Cloud
  Deployments](https://www.enterprisecloudcustomercouncil.com/docs/Cloud_Connectivity_and_DMZ_Architectures_Framework_Position_Paper.pdf)
  + "The Enterprise Cloud Customer Council (E3C) is a group of enterprise
    companies, primarily financial services, with the vision to become a leading
    voice for enterpriseorganizations in the pursuit of cloud interoperability,
    security,and portability with major cloud industry vendors and standards
    bodies.  The top cloud companies are closely involved and are actively
    assisting the E3C in achieving its goals.  Intel Corporation serves as
    facilitator for the group."
  + "A typical large scale enterprise compute environment provides resources and
    services to internal users and private B2B services to external users. As
    the organization shifts various compute resources to different cloud
    providers, the same controlled access techniques that existed in legacy Data
    Centers or Private Cloud deployments must be offered for these resources
    running in the public cloud.  This position paper is meant to give high
    level requirements to the CSPs and illustrate thechallenges experienced by a
    typical enterprise as it designs proper architecture to move workloads into
    the cloud utilizing IAAS model."
  + Challenges of Cloud Based DMZ Architectures
    * "A typical DMZ is a network virtualization schema when a particular
      network connects to at least two different networks with different
      security levels.  Security levels are defined as restrictions on
      connectivity access, so a DMZ is typically a network that has services
      that facilitate connectivity between networksof lesser access restrictions
      to network of greater connectivity restrictions."
  + See page-13, FIGURE 1: HYBRID CLOUD OVER VIRTUAL PRIVATE TRANSPORT
  + See page-14, FIGURE 2: HYBRID CLOUD PUBLIC TRANSPORT
  + Cloud DMZ Architectures
    * "A typical cloud DMZ is a connectivity domain, so each cloud is ultimately
      its own DMZ.  DMZscan be Layer 2 broadcast networks, Layer 3 IP networks
      and even networksutilizing various overlay protocols.  This chapter is
      primarily dedicated to identifying security boundaries and their
      relationship to network boundaries."
  + Borderless DMZ architecture
    * "Borderless DMZ is when all virtual compute instances are able to create
      connectivity domains directly between each other using some form ofoverlay
      networking.  Various forms of control systems may exist that program these
      overlays and insure that only authorized compute instances are able to
      interconnect.  With such a setup, the virtual compute host provides all
      the needed security, and the requirements for cloud gateway security
      become minimized.  At this point the security requirements for the cloud
      gateway may be reduced from controlling which other cloud networks can
      establish connectivity to just monitoring and from protecting from
      irregular traffic patterns.
    * "These gateways are special cases of tenant controlled Cloud Gateways typically deployed inside.The disadvantage of Borderless DMZ is the potential loss of network security hierarchy, and the scalabilityone has to give up by maintaining countless of potential overlay network tunnels.  Security hierarchy is not truly lost, but middle level of hierarchy would be moved closer to endpoint.  In case of maintaining overlay tunnels,the tunnels themselves are stateless and meant to set up almost as easily as additional TCP sessions."
    * "Borderless DMZ architecture is ultimately the one for the Zero Trust
      model. In such a model virtual network perimeters can be deployed on demand potentially creating connectivity domains on demand.  This architecture can be deployed as part of virtual compute instance security service and for those that trust the CSPs, it can be offered as a CSP service. Borderless DMZ architecture may appear to be the most overwhelming because it creates the illusion of many virtual connections set up between many virtualcompute nodes."
  + See page-21, FIGURE 6: BORDERLESS DMZS








## Articles

### 2021 


### 2020
- 2020-1221 [How to build a private cloud and why? | Parallels
  RAS](https://www.parallels.com/blogs/ras/how-to-build-a-private-cloud/)
  + "A private cloud involves a private network that accepts connections from
    internet-based clients. Businesses must not compromise security in this
    process. This is why a demilitarized zone (DMZ) is set up between the public
    network and the company’s private network."

- 2020-01-13 [Prepare your data center for a hybrid cloud
  strategy](https://searchcloudcomputing.techtarget.com/tip/Prepare-your-data-center-for-a-hybrid-cloud-strategy), Tom Nolle, President, CIMI Corporation
  + "A good hybrid cloud strategy assumes that the public cloud provides
    front-end application support, including information support designed to
    stimulate or enhance a transactional application. The transactional
    application is most likely to run in the data center, which means the data
    center has to expose APIs to which a cloud front end can reasonably
    connect."
  + "The first step is to define, secure and expose the proper APIs to link the
    cloud and data center. Think of this hybrid cloud boundary as a
    demilitarized zone (DMZ), a place that has its own rules, but also has to
    support both worlds and in some cases be a part of each one. These APIs are
    the border in the middle of the DMZ."




### 2019 

- [Designing Hybrid Cloud Architecture for the
  Future](https://www2.deloitte.com/content/dam/Deloitte/us/Documents/process-and-operations/us-designing-hybrid-cloud-architecture-for-the-future.pdf)
  + See page-4, re: EXHIBIT 3 | MICROSOFT HYBRID CLOUD REFERENCE ARCHITECTURE

- 2019-02-14 PC Mag: [Is the DMZ Dead? Not
  Quite](https://www.pcmag.com/news/is-the-dmz-dead-not-quite)
  + "If you've still got a DMZ in operation, then you'll find it's a typical
    example of network segmentation"
  + "Look closely and you'll generally find some combination of firewalls and
    routers. In most cases, the DMZ will be created by an edge security device
    (usually a firewall) that's then backed up by another router or firewall
    guarding the gates to the internal network."
  + "If you apply the DMZ mechanism on an entirely internal basis, then there
    are still use cases that makes sense. One example is protecting access to
    valuable data stores, access control lists, or similar treasure troves;
    you'll want any potential unauthorized users to jump through as many
    additional hoops as possible before they gain access."
  + "By adding this extra in-between network, you can implement additional
    security layers that malcontents will need to defeat before they can get to
    your actual internal network—where everything is presumably also covered not
    only by network access controls but endpoint protection suites, too."

- 2019-01-31 PC Mag: [Beef Up Security and Performance With Network Segmentation](https://www.pcmag.com/news/beef-up-security-and-performance-with-network-segmentation)
  + "There are several reasons for network segmentation; the most important
    reason is security. If your network is divided into several smaller
    networks, each with its own router or Layer 3 switch, then you can restrict
    entry to certain parts of the network. This way, access is only granted to
    endpoints that need it."
  + "...the Target breach in 2013. Attackers using credentials from the Heating,
    Ventilation, and Air Conditioning (HVAC) contractor had access to the
    point-of-sale (POS) terminals, the credit card database, and everything else
    on the network. Clearly, there was no reason for an HVAC contractor to have
    access to anything but the HVAC controllers, but they did because Target
    didn't have a segmented network."
  + "Logical segmentation would use virtual LANs (VLANs) or network addressing
    to accomplish the segmentation. Logical segmentation can be based on VLANs
    or specific subnets to define networking relationships or you may use both."


### 2018

- 2018-11-21 [Security in the Public Cloud — Roll your own DMZ on AWS, Azure or Google
  Cloud](https://medium.com/public-cloud-security/security-in-the-public-cloud-roll-your-own-dmz-on-aws-azure-or-google-cloud-d90598fbda28)

- 20281-06-18 [Virtual DMZs in the Cloud](https://resources.infosecinstitute.com/topic/virtual-dmzs-cloud/)

- 2018-06-01 [Is the DMZ dead in the Cloud?](https://www.linkedin.com/pulse/dmz-dead-cloud-neil-cavanagh/)
  + "Within the data centre, DMZ’s were traditionally used to host front end
    internet facing services such as web sites, email filters and remote access
    solutions. DMZ’s provide a great way to segment parts of a network so
    applications and systems can run within a self-contained environment."
  + "Azure VNETS provide a neat way to isolate services from each other and allow network aware services to deployed into a private network. You can deploy many types of Azure resources including virtual machines, kubernetes clusters and app services."
  + "Multiple subnets can deployed within a VNET so you can segment different
    types of resources within your virtual network, you can also direct traffic
    out of a subnet towards a virtual firewall appliance to almost mimic the
    traditional set up you have in a data centre."
  + "Azure can still offer you the same multi-layered protection as you may have
    in your on premise network, but it’s worth spending a bit of time evaluating
    the use of your applications and services before migrating them across"





### 2016

- 


### 2014 
- 2014-08-27
  [Three security practices that IoT will disrupt](https://www.networkworld.com/article/2599231/three-security-practices-that-iot-will-disrupt.html)
  + "It is accepted best practice in larger organizations to use DMZ network
    segments to isolate outbound traffic emitters, including web proxies for all
    internally-initiated web traffic and email relays for all
    internally-composed email messages. IoT devices disrupt this model in
    several ways."
  + "To defend against behavior that challenges established DMZ, proxy and relay
    practices, device capabilities must be researched before they are purchased."
  + "As we saw, IoT devices will disrupt three well-established security practices, but only one is likely to fall permanently into the dustbin of history."
    * SHAKEN BUT SAFE: Using DMZs, web proxies and email relays.
    * SHAKEN BUT SHOULD EVENTUALLY BE SAFE: Using centralized credential management.
    * SHAKEN AND FALLING: Using one big Internal Network behind a firewall.


### 2008 

- 2008-01-16 [Does virtualization spell the end of good DMZ security?](https://www.networkworld.com/article/2350433/does-virtualization-spell-the-end-of-good-dmz-security-.html)
