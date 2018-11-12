
Microservices Notes
==============================

### Concepts/Patterns 
* Google: Design patterns for container-based distributed systems
  * https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45406.pdf 
    * Single-Container Management Patterns
    * Single-node, multi-container application patterns
      * Sidecar pattern
      * Ambassador pattern
      * Adapter pattern 
    * Multi-node application patterns 
      * Leader-election pattern
      * Work queue pattern
      * Scatter/gather pattern 

* https://kubernetes.io/blog/2015/06/the-distributed-system-toolkit-patterns/

* Sidecar: "An application is deployed alongside each microservice that you have developed and deployed to a server/hosting instance. ... A sidecar runs alongside your service as a second process and provides 'platform infrastructure features' exposed via a homogeneous interface such as a REST-like API over HTTP."
  * source: 
  * https://docs.microsoft.com/en-us/azure/architecture/patterns/sidecar
  * https://blog.davemdavis.net/2018/03/13/the-sidecar-pattern/
  * https://www.abhishek-tiwari.com/a-sidecar-for-your-service-mesh/
  * https://dzone.com/articles/microservices-sidecar-pattern-implementation-using-1
  * http://blog.christianposta.com/microservices/00-microservices-patterns-with-envoy-proxy-series/
  * https://developer.ibm.com/code/2017/05/22/polyglot-microservices-and-the-sidecar-pattern/
  * https://medium.com/netflix-techblog/prana-a-sidecar-for-your-netflix-paas-based-applications-and-services-258a5790a015
  * https://blog.turbinelabs.io/the-first-step-in-modern-networking-isnt-a-sidecar-ed657db67cd3 
  * https://www.thoughtworks.com/radar/techniques/sidecars-for-endpoint-security
  * https://blog.openshift.com/kerberos-sidecar-container/


### Frameworks & Tooling
* Envoy 
  * https://www.envoyproxy.io/
    * "Originally built at Lyft, Envoy is a high performance C++ distributed proxy designed for single services and applications, as well as a communication bus and “universal data plane” designed for large microservice “service mesh” architectures. Built on the learnings of solutions such as NGINX, HAProxy, hardware load balancers, and cloud load balancers, Envoy runs alongside every application and abstracts the network by providing common features in a platform-agnostic manner. When all service traffic in an infrastructure flows via an Envoy mesh, it becomes easy to visualize problem areas via consistent observability, tune overall performance, and add substrate features in a single place."

* Istio
  * https://istio.io/
    * "Istio makes it easy to create a network of deployed services with load balancing, service-to-service authentication, monitoring, and more, without any changes in service code. You add Istio support to services by deploying a special sidecar proxy throughout your environment that intercepts all network communication between microservices, then configure and manage Istio using its control plane functionality, which includes:"
      * "Automatic load balancing for HTTP, gRPC, WebSocket, and TCP traffic."
      * "Fine-grained control of traffic behavior with rich routing rules, retries, failovers, and fault injection."
      * "A pluggable policy layer and configuration API supporting access controls, rate limits and quotas."
      * "Automatic metrics, logs, and traces for all traffic within a cluster, including cluster ingress and egress."
      * "Secure service-to-service communication in a cluster with strong identity-based authentication and authorization."
    * Istio uses an extended version of the Envoy proxy. Envoy is a high-performance proxy developed in C++ to mediate all inbound and outbound traffic for all services in the service mesh. Istio leverages Envoy’s many built-in features, for example:"=
      * "Dynamic service discovery"
      * "Load balancing"
      * "TLS termination"
      * "HTTP/2 and gRPC proxies"
      * "Circuit breakers"
      * "Health checks"
      * "Staged rollouts with %-based traffic split"
      * "Fault injection"
      * "Rich metrics"
    * https://istio.io/docs/concepts/policies-and-telemetry/
    * https://istio.io/docs/concepts/traffic-management/#pilot-and-envoy
    * https://istio.io/docs/concepts/security/
    * 

### Interesting Articles
* 2018 
* 2017
  * https://www.infoq.com/news/2017/01/production-ready-microservices
  * https://www.theregister.co.uk/2017/05/24/google_lyft_ibm_mix_microservices_into_management_mesh/
* 2016 
* https://www.susanjfowler.com/blog/2016/12/18/the-four-layers-of-microservice-architecture

