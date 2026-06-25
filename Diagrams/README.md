
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
  + Realtime (e.g., API, Web Services, database connection, ...)

- **Dotted**
  + Manual process
  + User performing a task through a UI
  + User uploading a file through a UI


### Line Color (e.g., data classification)
- In the case of a mixed use integration path, pick the color that represents the highest security classification

- **Dark Green**
  + Financial transactions

- **Red**
  + Senstive Data
    * Personally Identifiable Informaiton (PII)
    * HIPAA
    * etc. 

- **Blue**
  + Other regular transaction data      

- **Black**
  + Reference Data 


## References


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


