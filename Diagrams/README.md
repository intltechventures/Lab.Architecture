
# Architecture Drawing Resources

## Notation Conventions
   
_'''illustrative, not exhaustive'''_   


### Line Style (e.g., access mechanism, communications protocol, ...)

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


### Line Color (e.g., data classification)
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



## References

### Data Classificiation References    
(illustrative, not exhaustive)    


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



### Diagramming Speifications 
- ArchiMate
  + https://publications.opengroup.org/standards/archimate
    * [ArchiMate® 3.2 Specification](https://pubs.opengroup.org/architecture/archimate32-doc/index.html)


- C4 model 
  + https://c4model.com/ 
    * https://c4model.com/diagrams
    * https://c4model.com/tooling


- UML 
  + https://www.omg.org/spec/UML



### Icon Collections

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

### Suggested Books
 
- [Communication Patterns: A Guide for Developers and Architects, 1st Edition](https://www.amazon.com/Communication-Patterns-Guide-Developers-Architects/dp/1098140540/), (2023)


## EA Tools, with shared repository capabilities 

### EA Tools - Suggested

- Sparx Enterprise Architect (EA)
  + https://sparxsystems.com/


### EA Tools - Suggsted Alternatives

- Alfabet
  + https://www.alfabet.com/

- Bizzdesign 
  + https://bizzdesign.com/

- Mega Hopex
  + https://www.mega.com/

- SAP LeanIX 
  + https://www.leanix.net/

- ServiceNow EA
  + https://www.servicenow.com/products/enterprise-architecture.html
  + https://www.servicenow.com/products/strategic-portfolio-management


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


### Achitecture Diagramming Tools - Primary Suggestions

- Excalidraw
  + https://excalidraw.com

- LucidChart
  + https://lucidchart.com

- Microsoft 365 Visio 
  + https://www.microsoft.com/en-us/microsoft-365/visio

- Miro 
  + https://miro.com


### Architecture Diagramming Tools - Alternative Suggestions

- archimatetool.com 
  + https://www.archimatetool.com


- c4model.com
  + https://c4model.com


- d2lang.com
  + https://d2lang.com


- Diagrams.net
  + https://www.diagrams.net


- eventcatalog.dev
  + https://www.eventcatalog.dev


- icepanel.io
  + https://icepanel.io


- ilograph.com
  + https://ilograph.com


- likec4.dev
  + https://likec4.dev


- Omnigraffle
  + https://www.omnigroup.com/omnigraffle


- Structurizer
  + https://structurizr.com
  + https://github.com/orgs/structurizr/repositories
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

- PlantUML
  + https://plantuml.com
  + https://github.com/awslabs/aws-icons-for-plantuml


- Mermaid.js 
  + https://mermaid.js.org
    * See: Confluence plugin


### Diagrams-as-Code Tools - Secondary Suggestions

- https://eraser.io

- https://diagrams.mingrammer.com

- https://github.com/pistazie/cdk-dia

- https://github.com/mhlabs/cfn-diagram

- https://github.com/cycloidio/inframap

- https://grucloud.com

- https://www.pluralith.com


### Visual Diagramming Tools

- https://lucidscale.com/product/aws

- https://creately.com

- https://www.gliffy.com

- https://cacoo.com/features

- https://www.cloudcraft.co

- https://docs.fugue.co/visualization.html

- https://www.cloudockit.com

- https://app.cloudviz.io


### AI-Augmented Diagramming

- ChatGPT Canvas 

- Claude Artifacts

- Google AI Studio

- https://app.eraser.io

- https://excalidraw.com


