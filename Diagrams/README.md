
# Architecture Diagram Resources
           
**Status**: ```2026-08-15 I am reworking some of the organization of the content, adding new entries, and doing some judicious pruning.```    
             
                 
I am frequently involved in helping clients research, select, and adopt tools for the creation and maintenance of Enterprise Architecture and Solution Architecture artifacts – which frequently involves developing diagrams of various types.    
   
Such tools are often the cornerstone for establishing **GOVERNANCE** processes.    
   
At the lowest level of sophistication, you will often find teams creating and maintaining diagrams directly in something like PowerPoint (oh, the **HORROR**), or some other simple drawing tool.  Usually with each user independently maintaining ther own diagrams on their local machines (rarely will you ever find any centralized folder structures, _that are well-maintained_, to organize and share artifacts). There is a **tragic level of inefficiency** in maintaining such randomly distributed collections of artifacts – and there is no way to ensure that you have found the latest (or all) of the possible variations/instances. Reuse is impossible to achieve and maintain.    
   
At the highest level of sophistication, you may find teams using enterprise-class tools that allow for the **reuse of a single shared repository**, with automated sync with a Configuration Management Database (CMDB, such as ServiceNow), automated discovery of elements (third-party \*aaS, cloud services, network devices, routers, gateways, databases, servers, applications, integration flows, communication paths, etc.), and automated generation/update of diagrams based on changing relationship meta data that is captured in an enterprise model. Advanced solutions will usually include the ability to generate/export and perform some form of live integration of artifacts (e.g., lists, diagrams, reports, design documents, roadmaps, traceability maps, heat maps, capability models, reference archtiectures, patterns, policies, standards, specifications, etc.).        
       
The spectrum of available features/capabilities is quite wide, and continues to grow.       

The Achilles Heel of all such sophisticated tools? Initial costs (acquisition, training, implementation), and long-term maintenance costs (effort, resources, budgets).   
    
The unqiue dynamics (and constraints) at play within your organization will often severely limit your choices.    
   
This document is intended as a placeholder to collect and organize notes on a broad range of possible solutions.     
**It is not intended to be exhaustive, only illustrative.**      
   
_Caveat Emptor_ is still sound advice. Your own **Due Diligence** is always necessary.    



## Possible Diagram Notation Conventions To Consider

In almost every organization, I have found either no formal standard/guidance on diagram notation conventions, or lax adoption of any. This tends to create an environment for a wide range of variations (at best), and potential chaos (at worst). It also hinders effective communication, precision, accuracy, and reuse.    
    
The following are just _some suggested ideas_ to help stimulate discussion within an organization, and reflects some of my own personal thoughts/preferences.    
       
_'''illustrative, not exhaustive'''_      


### Line Style Convention (e.g., access mechanism, communications protocol, integration style, ...) Suggestions: 

+ **Solid**
  + Automated File Transfer (e.g., SFTP, ...)
  + Email delivery with attachments
  + File Sharing services 
  + ... 


- **Dashed**
  + Realtime (e.g., APIs, Web Services, direct database connection, ...)


- **Dotted**
  + Manual process
  + User performing a task through a UI
  + User uploading a file through a UI


### Line Color Convention (e.g., data classification, business criticality, ...) Suggestions: 
- In the case of a mixed use integration path, pick the color that represents the highest security classification


- **Red**
  + **Data Classifications**: ```Highly Restricted``` | ```Restricted (Highly Confidential)``` | ```Secret``` | ```Top Secret```
  + Senstive Customer, Employee, or Corporate Data
    * Personally Identifiable Informaiton (PII)
    * Private/Protected Personal Information (PPI)
    * HIPAA
    * Secret
    * etc. 


- **Blue**
  + **Data Classifications**: ```Confidential``` | ```Restricted``` | ```Confidential```
  + Transaction data      
  + Data integrations
  + Integrations, or flows, that do not meet any of the the other Line Color selection criteria


- **Dark Green**
  + **Data Classifications**: ```High Risk``` | ```Restricted``` | ```Confidential``` 
  + Financial transactions
  + Payment Card Industry (PCI) transactions 


- **Black**
  + **Data Classifications**: ````Private``` | ```Sensitive``` | ```Internal Only```
  + Private Company Reference Data 
  + Non-public Reference Data 
  + Memos, intellectual property, and email messages


- **Gray/Grey**
  + **Data Classifications**: ```Public``` | ```Unclassified``` | ```Open Data```
  + Publicly available informaiton 
  + Public Reference Data 

### Line Thickness Convention (e.g., max data size, peak transaction volume, ...) Suggestions: 

The Width Factor is intended to represent a ```relative value```, depending the capabilities supported by your selected tool.

- Width Factor: 1
  + Low volume | size 

- Width Factor: 2
  + Med volume | size

- Width Factor: 3
  + High volume | size
  




## References

### Data Classification References    

When developing standard conventions for enterprise-wide visual diagram modeling, there should be clear identification of the *data classification* for each data source/target, and integration flow. This can be especially important when there may be imminent threats that require immediate mitigation, or remediation. 
   
_```illustrative, not exhaustive```_


- https://www.ibm.com/think/topics/pii


- NIST SP 1800-39 Data Classification Practices
  + https://csrc.nist.gov/pubs/sp/1800/39/ipd


- https://www.ignyteplatform.com/blog/nist/data-classification-nist-levels/


- AWS Data classification models and schemes
  + https://docs.aws.amazon.com/whitepapers/latest/data-classification/data-classification-models-and-schemes.html


- https://www.cyera.com/blog/four-levels-of-data-classification


- https://www.paloaltonetworks.com/cyberpedia/data-classification


- Payment Card Industry Data Security Standard (PCI DSS) 
  + https://en.wikipedia.org/wiki/Payment_Card_Industry_Data_Security_Standard
  + https://www.pcisecuritystandards.org/standards/


- PCI DSS Data Classification Requirements
  + https://pcidssguide.com/pci-dss-data-classification-requirements/


- https://www.proofpoint.com/us/threat-reference/data-classification


- https://www.umsystem.edu/departments-staff/information-technology/data-protection-security/data-classification



### Formal Diagram Notation Specifications 
   
_```illustrative, not exhaustive```_
     

- ArchiMate
  + https://en.wikipedia.org/wiki/ArchiMate
  + https://publications.opengroup.org/standards/archimate
  + https://publications.opengroup.org/archimate-library
    * [ArchiMate® 3.2 Specification](https://pubs.opengroup.org/architecture/archimate32-doc/index.html)
   
   
- C4 model (Context, Container, Component, Code)
  + https://en.wikipedia.org/wiki/C4_model
  + https://c4model.com/ 
    * https://c4model.com/diagrams
    * https://c4model.com/tooling
   
   
- Unified Modeling Langauge (UML)
  + https://en.wikipedia.org/wiki/Unified_Modeling_Language
  + https://www.omg.org/spec/UML
  + [v2.5.1](https://www.omg.org/spec/UML/2.5.1/PDF)


### Icon Collections
   
_```illustrative, not exhaustive```_   
   
   

- Misc. Icons
  + https://fontawesome.com/versions
    * https://fontawesome.com/icons
    * https://fontawesome.com/search?ic=free
    * https://fontawesome.com/v6/icons


- Cloud icons
  + AWS
    * https://aws.amazon.com/architecture/icons/

  + Azure 
    * https://learn.microsoft.com/en-us/azure/architecture/icons/

  + Google CGP
    * https://cloud.google.com/icons?hl=en

  + Oracle OCI 
    * https://docs.oracle.com/en-us/iaas/Content/General/Reference/graphicsfordiagrams.htm

  + ServiceNow
    * https://developer.servicenow.com/dev.do#!/reference/next-experience/orlando/now-components/now-icon/gallery



## Suggested Background Reading
   

_```illustrative, not exhaustive```_

    

### Suggested Books   
    
- [Communication Patterns: A Guide for Developers and Architects, 1st Edition](https://www.amazon.com/Communication-Patterns-Guide-Developers-Architects/dp/1098140540/), (2023)   
   
- [The C4 Model: Visualizing Software Architecture](https://www.amazon.com/dp/B0GC5YKYFD), (2026)   



## EA Tools, with shared repository capabilities 

_```illustrative, not exhaustive```_

- **Pros:**
  + Holistic view
  + Single repository
  + Accuracy
  + Abundance of features
  + Sophisticated capabilities    
   
    
- **Cons:**
  + Costs
  + Complexity
  + Maintenance effort
  + Constraints/limitations of their product roadmap    
   
   
### EA Tools, Industry Analyst Reports

- Gartner Magic Quadrant (MQ) for Enterprise Architecture Tools
  + https://www.gartner.com/en/documents/7015598
    * 2026 Report (courtesy copy download from Ardoq)
      * https://content.ardoq.com/gartner-magic-quadrant-for-enterprise-architecture-tools


- The Forrester Wave™: Enterprise Architecture Management Suites
  + https://www.forrester.com/blogs/category/enterprise-architecture/
  + https://www.forrester.com/research/wave/
    * 2025-Q4 Report
      * https://www.forrester.com/report/the-enterprise-architecture-management-suites-landscape-q4-2025/RES190110
        * https://www.forrester.com/blogs/the-enterprise-architecture-management-suites-landscape-q4-2025-is-out/
   
      

### EA Modeling Tools - Suggested


- Bizzdesign 
  + https://bizzdesign.com/
  + https://bizzdesign.com/transformation-suite/unify
  


- Sparx Enterprise Architect (EA)
  + https://sparxsystems.com/
  + https://sparxsystems.com/products/ea/
  + https://sparxsystems.com/products/ea/compare-editions.html
  + https://sparxsystems.com/products/ea/shop/   
      
  + [Sparx EA Forum](https://sparxsystems.com/forums/smf/)
    * [Forum: General Board](https://sparxsystems.com/forums/smf/index.php/board,26.0.html)
    * [Forum: Latest News](https://sparxsystems.com/forums/smf/index.php/board,22.0.html)
    * [Forum: Suggestions and Requests](https://sparxsystems.com/forums/smf/index.php/board,27.0.html)
    * [Forum: Bugs and Issues](https://sparxsystems.com/forums/smf/index.php/board,25.0.html)
    * [Forum: Automation Interface, Add-Ins and Tools](https://sparxsystems.com/forums/smf/index.php/board,23.0.html)
  + Resources: 
    * https://sparxsystems.com/resources/gallery/
  + MDG Extensions
    * https://sparxsystems.com/products/mdg/
  + Third-Party Extensions:
    * https://sparxsystems.com/products/3rdparty.html
      * https://sparxsystems.com/products/3rdparty.html#eaUtils
  + Icon Sets:
    * https://sparxsystems.com/enterprise-architect/cloud-architecture/icon-set.html
  + Free Downloads: 
    * https://sparxsystems.com/products/ea/downloads.html
      * See Image Library (2017-07-27)   
     
  + **Rationale**
    * Easier to get started 
    * Consider this your "training wheels" phase
    * Many EA tool initiatives fail after a few years (neglect, failure to sustain their budgets/staffing, ...)
  + **Pros:**
    * Low cost 
    * Ease of Use
    * Number of features included 
    * Offers floating license option
    * Professional Edition includes [icons for major cloud providers (AWS, Google, Azure)](https://sparxsystems.com/resources/webinar/sparxservices/cloud-architecture/)
  + **Cons:**
    * Rudimentary integration capabilities
    * The optional downloads available in the Image Library have not been updated since 2017. 
    


### EA Tools - Suggsted Alternatives
     
- ~~Alfabet~~
  + 2025-01-09: Bizzdesign Adds Alfabet Business Following Successful Closing of MEGA International Acquisition, Creating a New Force in the EA and Strategic Portfolio Management Markets
    * https://bizzdesign.com/press-releases/bizzdesign-adds-alfabet-business-following-successful-closing-mega-international



- Ardoq
  + READ THIS FIRST:
    * https://help.ardoq.com/en/articles/43993-ardoq-compared-to-drawing-modeling-and-data-visualization-tools
  + https://ardoq.com/
  + https://github.com/ardoq
  + https://twitter.com/ardoqCom
  + https://github.com/ardoq
  + https://www.glassdoor.com/Overview/Working-at-Ardoq-EI_IE2378970.11,16.htm

    
- Avolution Abacus
  + https://www.avolutionsoftware.com/abacus/
  + https://www.avolutionsoftware.com/abacus/frameworks/
  + https://www.avolutionsoftware.com/feature-comparison-enterprise-architecture-tool/
  + https://www.avolutionsoftware.com/our-resources/integrated-enterprise-architecture-diagrams/  
  + Also see:
    * https://www.avolutionsoftware.com/resources/
    * https://www.avolutionsoftware.com/abacus/dynamic-data-visualizations/
    * https://www.avolutionsoftware.com/solutions/application-rationalization/
    * https://www.avolutionsoftware.com/abacus/enterprise-architecture-modeling-roadmapping/    
   
    
- ~~Mega Hopex~~
  + 2024: [Acquired by Bizzdesign](https://bizzdesign.com/press-releases/bizzdesign-adds-alfabet-business-following-successful-closing-mega-international)
  + 2024-09-05: https://main.nl/press-release/bizzdesign-acquires-mega/
    * "_Main Capital Partners-backed Bizzdesign acquired MEGA International and its flagship HOPEX platform. This deal combined two major enterprise architecture (EA) and digital transformation software leaders, continuing under the Bizzdesign brand. Shortly after, Bizzdesign also integrated Alfabet to form a unified product suite._" 
    

- OrbusSoftware > OrbusInfinity
  + https://www.orbussoftware.com/
  + https://www.orbussoftware.com/capability/central-repository
  + https://www.orbussoftware.com/capability/frameworks-and-standards
  + https://www.orbussoftware.com/capability/enterprise-architecture-diagramming
  + https://www.orbussoftware.com/capability/integrations
  + https://www.orbussoftware.com/capability/dashboards-reporting
  + https://www.orbussoftware.com/capability/it-landscape-visualization
    
   
- SAP LeanIX
  + https://www.leanix.net/en/
  + https://en.wikipedia.org/wiki/LeanIX
  + 2023-09-07: [LeanIX acquired by SAP](https://www.linkedin.com/feed/update/urn:li:activity:7105442685317959680/)
   
   
- ServiceNow EA
  + https://www.servicenow.com/products/enterprise-architecture.html
  + https://www.servicenow.com/products/strategic-portfolio-management
  + Also see:
    * https://www.servicenow.com/products/application-portfolio-management.html
    
    
- ~~Software AG > ARIS ((Architecture of Integrated Information Systems)~~
  + https://www.softwareag.com/en/
  + 2025-01-08: Software AG retrenches to its core ARIS process management and A&N mainframe tools
    * https://diginomica.com/software-ag-retrenches-aris-adabas-natural
  +     

## Simplistic Diagramming Tools 

- **Pros**
  + Typically lower costs than formal EA tools licensing arrnagements
  + Ease of use 

- **Cons**
  + Frequently the per-user subscription pricing becomes untenable, at scale 
  + Frequently does not support the complete specification of some formal diagramming notations (e.g., UML, Arhimate, etc.) 
  + Typically do not support defining reusable shared element/component definitions
  + Typically has very poor reuse across diagrams 
  + Usually does not support an enterprise-wide shared repository 


### Simple Achitecture Diagramming Tools - Primary Suggestions
   
_```illustrative, not exhaustive```_

- Miro 
  + https://miro.com


### Simple Architecture Diagramming Tools - Alternative Suggestions
   
_```illustrative, not exhaustive```_
    
    
- Archi 
  + https://www.archimatetool.com



- c4 modeling
  + https://c4model.com
  + https://c4model.com/tooling



- Creately 
  + https://creately.com
  + https://creately.com/tour/
  + https://creately.com/enterprise/
  + https://www.gliffy.com/products/confluence/zero-egress
  + https://creately.com/lp/onprem-services/



- d2lang.com
  + https://d2lang.com


- Diagrams.net (previously known as draw.io)
  + https://en.wikipedia.org/wiki/Diagrams.net
  + https://www.diagrams.net
    * https://app.diagrams.net/
  + https://www.drawio.com/
  + https://github.com/jgraph/drawio
    * License: Apache 2.0 
    * 98.5 JavaScript 
  

- eventcatalog.dev
  + https://www.eventcatalog.dev


- Excalidraw
  + https://excalidraw.com/
    * "_Excalidraw is a virtual collaborative whiteboard tool that lets you easily sketch diagrams that have a hand-drawn feel to them._"


- Gliffy 
  +  https://www.gliffy.com
  + https://help.gliffy.com/
    + https://help.gliffy.com/online/Content/GliffyOnline/home-gliffy-online.htm
  + https://www.gliffy.com/pricing
  + https://www.gliffy.com/products/confluence
    

- icepanel.io
  + https://icepanel.io
    * "_Collaborative diagramming and modelling tool for software architecture_"
  + https://icepanel.io/the-icepanel-loop
  + https://docs.icepanel.io/getting-started
  

- ilograph.com
  + https://ilograph.com
  + https://www.ilograph.com/pricing.html
  + https://www.ilograph.com/docs/index.html
    * https://www.ilograph.com/docs/spec/
  + https://www.ilograph.com/features.html
    * See: "_Collaboration and sharing options vary depending on environment_"
      * https://www.ilograph.com/team.html
        * "_With a team workspace, your team's diagrams are centralized and always available in the cloud._"
        * Note: The appears to be a simple storage approach (i.e., still separate diagrams), not semantically linked / stored in a holistic repository. 
      * https://www.ilograph.com/desktop/index.html
      * https://marketplace.atlassian.com/apps/1229877/ilograph-interactive-diagrams-for-confluence


- likec4.dev
  + https://likec4.dev
    * "_Architecture as Code - Describe your system architecture with code._"
  + https://likec4.dev/#features
  + https://likec4.dev/tutorial/
  + https://github.com/likec4/likec4/discussions
  + https://github.com/likec4/likec4
    * License: MIT 
    * 97.5% TypeScript     
    

- Omni Group > OmniGraffle
  + https://www.omnigroup.com/
  + https://www.omnigroup.com/omnigraffle
  + https://www.omnigroup.com/omnigraffle/specs/
  + https://www.omnigroup.com/omnigraffle/features/
  + https://www.omnigroup.com/omnigraffle/buy
    * Mac, iPad, iPhone 


- Structurizer
  + https://structurizr.com
    * See: [Introducing Structurizr vNext](https://www.patreon.com/Structurizr/posts/introducing-146923136)
  + https://docs.structurizr.com/
    * https://docs.structurizr.com/quickstart    
    * https://docs.structurizr.com/features
    * https://docs.structurizr.com/getting-started
    * https://docs.structurizr.com/commands
    * https://docs.structurizr.com/dsl
    * https://docs.structurizr.com/ai
  + https://github.com/orgs/structurizr/repositories
    * https://github.com/structurizr/structurizr
      * License: Apache 2.0 
      * 59.7% Java 
      * 37.6% JavaScript       
  + https://www.patreon.com/Structurizr/posts/cloud-service-of-142577083
    * NOTE: "_Structurizr cloud service will reach its End of Life (EOL) on 30 September 2026._"
    * "_The cloud service was launched in 2015 as a way to render and publish diagrams created with the Structurizr for Java library. Although the cloud service has seen some good usage over the past 10 years, engineering teams have consistently been reluctant to publish their software architecture diagrams to the cloud. This ultimately resulted in the creation of the self-hosted Structurizr on-premises installation and Structurizr Lite products, both of which were open sourced in early 2023. Cloud service usage has since steadily declined, and the decision to shutdown the cloud service will allow us to better focus on the self-hosted products moving forward._"
    * Timeline: 
      * 31st December 2025: Last date for new account sign ups.
      * 1st April 2026: Workspaces owned by free accounts will become read-only.
      * 1st July 2026: All workspaces will become read-only; all remaining monthly subscriptions will be stopped.
      * 30 September 2026: Cloud service shutdown.    
   + https://www.patreon.com/Structurizr/posts/introducing-146923136
     * "_The first announcement is that everything is being consolidated into a single Structurizr tool and a single git repo:_"
       * https://github.com/structurizr/structurizr
       * https://docs.structurizr.com/
         * https://docs.structurizr.com/binaries
           * "_All Structurizr commands are free to use from these binaries except for server, which requires a license_"
             * https://docs.structurizr.com/server/pricing
     * https://github.com/structurizr/java     
         * "_This repository was archived by the owner on Mar 28, 2026. It is now read-only._"         
         * https://docs.structurizr.com/java 
     * "_The current version of the Structurizr on-premises installation is a traditional Java EE web application, which requires deployment into a web server such as Apache Tomcat if you're not using the prebuilt Docker image. The new version of the tooling moves everything to Spring Boot with an embedded version of Apache Tomcat, much like the current version of Structurizr Lite. This provides a consistent approach to using Structurizr, regardless of which product you are using._"
     * "_Using the Structurizr server via the prebuilt binaries requires a license._"
       * https://docs.structurizr.com/server/pricing



- tldraw.dev
  + https://tldraw.dev



## AI-enabled Drawing Tools 

- Eraser.io 
  + https://eraser.io/
  + https://www.eraser.io/solutions/enterprise-architects
  + https://www.eraser.io/product/ai-diagrams
  + https://www.eraser.io/product/diagramming-api
  + https://www.eraser.io/product/integrations
  

- LucidChart
  + https://lucidchart.com
  + https://lucid.co/create/aws-architecture-diagram-software


- Microsoft 365 Visio 
  + https://www.microsoft.com/en-us/microsoft-365/visio
    * https://www.microsoft.com/en-us/microsoft-365/visio/visio-plans-and-pricing
  

## Diagrams-as-Code Tools

- **Pros**
  + Automated diagram build
  + Can be integrated into build pipelines/processes
  + Efficient to regenerate all diagrams


- **Cons**
  + No visual UI design capability
  + No shared repository of artifact/element definitons
  + Poor/limited reuse (cumbersome and manually intensive, at best)
  + Manually intensive to define 
  + Definitions can be automated, if there is a highly detailed/accurate set of meta data defining elements and their relationships/attributes


### Diagrams-as-Code Tools - Primary Suggestions
    
_```illustrative, not exhaustive```_

- GraphViz 
  + https://graphviz.org/
  + https://graphviz.org/documentation/
  + https://graphviz.org/resources/
  + https://gitlab.com/graphviz/graphviz
    * License: Eclipse Public License - v 2.0    
   
   
- PlantUML
  + https://en.wikipedia.org/wiki/PlantUML
  + https://plantuml.com
  + https://plantuml.com/sitemap
  + https://plantuml.com/news
  + https://plantuml.com/starting
  + https://plantuml.com/stdlib
  + https://plantuml.com/download
  + https://forum.plantuml.net/
  + https://plantuml.com/guide (PDF)
  + https://crashedmind.github.io/PlantUMLHitchhikersGuide/
  + https://github.com/awslabs/aws-icons-for-plantuml
  + https://github.com/plantuml
    * https://github.com/orgs/plantuml/repositories?type=all
    * https://github.com/plantuml/plantuml-stdlib
    * https://github.com/plantuml/clide
    * https://github.com/plantuml/plantuml-for-confluence
    * https://github.com/plantuml/plantuml
    * https://github.com/plantuml/plantuml-mcp
      * License: LGPL-3.0 (COPYING.LESSER), GPL-3.0 (LICENSE), GPL-3.0 (COPYING) 
      * 99.2% Java 


- Mermaid.js 
  + https://mermaid.js.org
    * See: Confluence plugin


### Diagrams-as-Code Tools - Secondary Suggestions
   
_```illustrative, not exhaustive```_
   
- TBD ...
 
      


## Automated Discovery / Generation of Diagrams 

_```illustrative, not exhaustive```_


- Cacoo 
  + https://cacoo.com/
  + https://cacoo.com/features
    * See: "_Use the AWS importer or code-to-graph to instantly turn infrastructure and code into clear, editable diagrams._"
  + https://nulab.com/pricing/cacoo/



- Cdk-dia
  + https://github.com/pistazie/cdk-dia
    * "_Cdk-dia diagrams your CDK provisioned infrastructure using the Graphviz dot language._"
    * License: MiT 
    * 96.1% JavaScript



- cloudcraft (by Datadog) 
  + https://www.cloudcraft.co
    * "_Automatically create AWS and Azure architecture diagrams in seconds_"
  + https://www.cloudcraft.co/solutions
    * "_Automatically produce real-time diagrams of your AWS and Azure architectures with Live Scanning. Through Live Scans_"
  + https://docs.datadoghq.com/cloudcraft/
  + https://docs.datadoghq.com/cloudcraft/api/
  + https://www.cloudcraft.co/security
  + https://www.cloudcraft.co/pricing 


- Cloudkit (by Lansweeper) 
  + https://www.cloudockit.com
    * "_Automatically generate architecture diagrams and technical documentation of your cloud environments_"
  + https://www.cloudockit.com/automated-editable-diagrams/
  + Integrations: 
    * https://www.cloudockit.com/cloud-aws/
    * https://www.cloudockit.com/cloud-azure/
    * https://www.cloudockit.com/cloud-gcp/
    * https://www.cloudockit.com/on-premise/



- Cloudviz.io 
  + "_Automatically generate live AWS architecture diagrams, access complete infrastructure history, and track changes — effortlessly_" 
  + https://docs.cloudviz.io/
  + https://cloudviz.io/developers
  + https://cloudviz.io/pricing
 
 
 
- ~~Fugue.co~~
  + 2022-02-17: [Snyk acquired Fugue](https://snyk.io/blog/snyk-welcomes-fugue-developer-first-cloud-security/)  
  + Founded: 2013 in Frederick, Maryland.
  + Core Focus: Cloud security posture management (CSPM) and policy-as-code automation for AWS, Azure, and Google Cloud.
  + Acquisition: Bought by developer security platform Snyk in February 2022 to expand its infrastructure-as-code security offerings.
  + https://snyk.io/
  + https://github.com/fugue
    * https://github.com/orgs/fugue/repositories
      * As of 2026-08-15: No updates to repositories since Sept 3, 2024


- GruCloud 
  + https://grucloud.com
    * "_GruCloud is a low/no-code infrastructure as a code tool. It can generate code from live infrastructure, and deploy resources to the cloud from code. Benefit from infrastructure as code without the hassle of manually authoring the infrastructure description._"
    * **Visualize the resources:**
      * "_The ```gc list --graph``` command displays a graph of the live infrastructure showing the dependencies between resources._"
      * "_he ```gc tree``` command displays a mindmap resources types._"
  + https://github.com/grucloud
  + https://github.com/grucloud/grucloud
    * Providers: 
      * https://github.com/grucloud/grucloud/blob/main/packages/providers/aws/README.md
      * https://github.com/grucloud/grucloud/blob/main/packages/providers/google/README.md
      * https://github.com/grucloud/grucloud/blob/main/packages/providers/azure/README.md
      * https://github.com/grucloud/grucloud/blob/main/packages/providers/k8s/README.md
    * License: GPL-3.0 
    * 99.8% JavaScript 
    * 2026-08-15: It appears this repository has not been updated since ~2024 
    
  

- inframap 
  + https://github.com/cycloidio/inframap
    * "_Read your tfstate or HCL to generate a graph specific for each provider, showing only the resources that are most important/relevant._"
    * "_We support all cloud providers, but we have some (listed below) that we have specific logic that allows us to better represent information that comes from these providers._"
    * License: MIT 
    * 97.2% Go 



- pluralith 
  + https://www.pluralith.com
    * "_Visualise Terraform Infrastructure, Directly from your Codebase._"
    * "_A tool for Terraform state visualisation and automated generation of infrastructure documentation_"
    * See Pricing: 
      * "_Flat-rate packages with flexible usage-based overflow pricing._"
      * "_How many terraform plan runs per month do you have?_"
      * "_Local Development, Free Forever_"
  + https://docs.pluralith.com/
  + https://github.com/Pluralith/pluralith-cli
    * License: MPL-2.0 
    * 98.5% Go 

 

## Diagram Drawing Libraries
    
_```illustrative, not exhaustive```_
    

- JoinJS
  + https://www.jointjs.com/
    * "_JointJS is a modern JavaScript library for visualization and interaction with diagrams and graphs. It can be used to create anything from static diagrams to fully interactive diagramming tools and application builders. JointJS is opensource, completely free to use, and our way of giving back to the community._"
      * https://github.com/clientIO/joint
        * [Mozilla Public License Version 2.0](https://github.com/clientIO/joint?tab=MPL-2.0-1-ov-file)
    * "_JointJS+ is the paid commercial extension to the JointJS Core Library. It builds on the JointJS foundation and widely extends its functionality by more than 40 components, implementing various UI widgets, interaction components, automatic layouts, control panels and other functionality, to build truly advanced visual applications._"
        * https://www.jointjs.com/license    
    * https://www.jointjs.com/about-us
    * https://www.jointjs.com/pricing
    * https://docs.jointjs.com/
    * https://www.jointjs.com/blog
    * https://www.youtube.com/@jointjs-library/
    * Reviews:
      * https://www.g2.com/products/jointjs/reviews
      * https://www.capterra.com/p/213029/Rappid/reviews/
      * https://www.softwareadvice.com/diagram/rappid-profile/reviews/
  + https://www.client.io/
    + "_Build Low-code tools that delight your customers._"
    + https://www.linkedin.com/company/client-io-s-r-o-/
      * "_client IO is the industry leader in diagramming solutions for the web era. Since 2011 our products have been enabling organizations to build web-based workflow, BPMN and flowchart diagramming products quickly and easily. client IO is the creator of JointJS and Rappid HTML 5 diagramming framework and our customers include Fortune 500 companies._"
    + https://www.glassdoor.com/Overview/Working-at-client-IO-EI_IE5046602.11,20.htm
      * https://www.glassdoor.com/Reviews/client-IO-Reviews-E5046602.htm



