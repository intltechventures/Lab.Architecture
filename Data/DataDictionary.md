
Data Dictionary Resources
====

In many instances, I've seen organizations purchase expensive/heavy-weight tools for the intended purpose of creating an Enterprise Data Dictionary - but, which is subsequently rarely (if ever) used by anyone outside of the data management team. 

This document is inteded as a collection of links to resources, and suggested ideas, for establishing and managing an Enterprise Data Dictionary - that can scale from the small, to the large. 

### Premise
* A modern data dictionary could/should be implemented using OWL/RDF standards, tooling. 


### Guiding Principles
* In general, the very concept of an Enterprise Data Dictionary is actually an anti-pattern. 
* The concept of a Data Dictionary is generally most applicable within a bounded context (e.g. as selected/defined for use in the design of a set of microservices)
* Leverage Code Standards (e.g. NCIC, AAMVA, ISO, ANSI, ...)


### Questions To Consider:
* Do you require the ability to ```Version``` a Data Dictionary entry?
* Who will be the consumers of your data dictioanary?
* How will you publish/share your data dictionary (to HTML? PDF? XML? RDF?)
* When should the following be used (see Footnote [1])?
  * Enumerations
    * "What rules should govern when to use enumeration types versus less contraining types?"
  * Code table references
    * Recommendation:
      * Defination of a Code should include a Source and Version (e.g. State Code="CA", Source="NCIC", veresion="2018")
  * Ranges
    * How to implement?
  * Numeric precision
    * How is precision defined?
    * HOw to represent precision?
  * Units:  
    * How to represent a distance measured in feet, inches, meters, centimeters, (and conversions for such)?
  * Partial Values
    * "Assuming this is necessary, how should the capability to exchange partial values be implemented?"  
    * "Example:  How to represent the following situation:  It is known that a phone number ends in `–3111` but the AreaCode and Prefix are unknown."
  * General null categories:  
    * "How to represent and unambiguously distinguish the following kinds of values:  unknown, none, N/A, nil or null value, etc.?"
* How should the following be handled?
  * Name/Value Property Tables



### General References/Concepts
* W3C RDF
  * https://en.wikipedia.org/wiki/Resource_Description_Framework
  * https://www.w3.org/RDF/
  * https://www.w3.org/2007/03/VLDB/
  * https://www.w3.org/wiki/SPARQL
    * "SPARQL is an RDF query language and protocol produced by the W3C RDF Data Access Working Group (DAWG). It was released as a W3C Recommendation in January of 2008."
  * https://www.w3.org/wiki/RDF_Query
  * https://www.w3.org/wiki/SPARQL/Extensions
* W3C OWL
  * https://en.wikipedia.org/wiki/Web_Ontology_Language
  * https://www.w3.org/OWL/
  * [W3 OWL Web Ontology Language Reference, ~2004](https://www.w3.org/TR/owl-ref/)
    * "The Web Ontology Language OWL is a semantic markup language for publishing and sharing ontologies on the World Wide Web. OWL is developed as a vocabulary extension of RDF (the Resource Description Framework) and is derived from the DAML+OIL Web Ontology Language"
  * https://www.w3.org/2001/sw/wiki/OWL/Implementations
* W3C OWL 2
  * [W3 OWL 2 Web Ontology Language Document Overview, ~2012](https://www.w3.org/TR/owl2-overview/)
  * "The OWL 2 Web Ontology Language, informally OWL 2, is an ontology language for the Semantic Web with formally defined meaning. OWL 2 ontologies provide classes, properties, individuals, and data values and are stored as Semantic Web documents. OWL 2 ontologies can be used along with information written in RDF, and OWL 2 ontologies themselves are primarily exchanged as RDF documents."
  * [W3C OWL 2 Web Ontology Language Quick Reference Guide ](https://www.w3.org/TR/owl2-quick-reference/)
  * [W3C OWL 2 Web Ontology Language Structural Specification and Functional-Style Syntax](https://www.w3.org/TR/owl2-syntax/)
  * [W3C OWL 2 Web Ontology Language New Features and Rationale](https://www.w3.org/TR/owl2-new-features/)
  * [W3C OWL 2 Web Ontology Language Primer ](https://www.w3.org/TR/owl2-primer/)
* [W3C Semantic Web Development Tools](https://www.w3.org/2001/sw/wiki/Tools)
* [DOD 8320.1-M Data Administration Procedures](http://www.dtic.mil/docs/citations/ADA343735)
  * 17 properties (class words) defined for a data element 
    * Amount		A monetary value
    * Angle:	    The rotational measurement between two lines and/or planes diverging from a common point and/or line.
    * Area: 	    The two-dimensional measurement of a surface expressed in unit squares.
    * Code: 	    A combination of one or more numbers, letters, or special characters substituted for a specific meaning.
    * Coordinate:	One of a set of values that identifies the location of a point.
    * Date: 		The notation of a specific period of time.
    * Dimension:  	A one-dimensional measured linear distance.
    * Identifier:	A combination of one or more numbers, letters, or special characters that designates a specific object and/or entity, but has no readily definable meaning.
    * Mass: 		The measure of inertia of a body.
    * Name:     	A designation of an object and/or entity expressed in a word or phrase.
    * Quantity:		A non-monetary numeric value.
    * Rate:     	A quantitative expression that represents the numeric relationship between two measurable units.
    * Temperature:	The measure of heat in an object.
    * Text:     	An unformatted character string generally in the form of words.
    * Time:     	A notation of a specified chronological point within a period.
    * Volume:   	A measurement of space occupied by a three-dimensional figure.
    * Weight:   	The force with which an object is attracted toward the earth and/or other celestial body by gravitation.
* [ISO/IEC Standard 11179 Specification and Standardization of Data Elements](https://en.wikipedia.org/wiki/ISO/IEC_11179)
  * http://metadata-standards.org/11179/ 




### RDF Type Tools / Exemplars
* https://github.com/timrdf/csv2rdf4lod-automation/wiki/Alternative-Tabular-to-RDF-converters
* https://curlie.org/docs/en/rdf.html
* Eionet Data Dictionary 
  * https://dd.eionet.europa.eu/searchelements
  * https://dd.eionet.europa.eu/schemasets/browse/
  * https://dd.eionet.europa.eu/vocabularies
  * https://dd.eionet.europa.eu/namespaces
* https://wiki.dbpedia.org/wiktionary-rdf-extraction
* http://www.rdfhdt.org/
  * "RDF/HDT is a project funded by the Spanish Ministry of Economy and Competitiveness (TIN2009-14009-C02-02); Science Foundation Ireland: Grant No. SFI/08/CE/I1380, Lion-II; Chilean Fondecyt’s 1110287 and 1-110066."
* SPARQL Implementations and Currently Active SPARQL Endpoints
  * https://www.w3.org/wiki/SparqlEndpoints
  * https://www.w3.org/wiki/SparqlImplementations


### OWL Type Tools / Exemplars
* [PREMIS OWL Ontology for PRMIS Data Dictionary v3](http://www.loc.gov/standards/premis/ontology/owl-version3.html)
  * Re: Library of Congress, Standards
  * http://www.loc.gov/standards/premis/ontology/
  * http://www.loc.gov/standards/premis/
    * "The PREMIS Data Dictionary for Preservation Metadata is the international standard for metadata to support the preservation of digital objects and ensure their long-term usability. Developed by an international team of experts, PREMIS is implemented in digital preservation projects around the world, and support for PREMIS is incorporated into a number of commercial and open-source digital preservation tools and systems. The PREMIS Editorial Committee coordinates revisions and implementation of the standard, which consists of the Data Dictionary, an XML schema, and supporting documentation."



### Other Exemplars
* City of Seattle, Integrated Library System (ILS) Data Dictionary 
  * https://catalog.data.gov/dataset/integrated-library-system-ils-data-dictionary
    * "This dataset is useful for understanding the codes used in some of Seattle Public Library's other datasets. These codes (namely "ItemType" and "ItemCollection") are systematically used in the cataloging of items within Integrated Library System (ILS), Horizon (Sirsidynix). 

  * https://catalog.data.gov/dataset/integrated-library-system-ils-data-dictionary/resource/34e24afb-cbe6-44f2-b06c-459d228a55fd
  * https://data.seattle.gov/api/views/pbt3-ytbc/rows.rdf?accessType=DOWNLOAD
* International Digital Object Identifier (DOI) Foundation
  * https://www.doi.org
    * "International DOI Foundation (IDF), a not-for-profit membership organization that is the governance and management body for the federation of Registration Agencies providing Digital Object Identifier (DOI) services and registration, and is the registration authority for the ISO standard (ISO 26324) for the DOI system. The DOI system provides a technical and social infrastructure for the registration and use of persistent interoperable identifiers, called DOIs, for use on digital networks."
  * https://www.doi.org/doi_handbook/4_Data_Model.html
    * The DOI data model has three tools to support its metadata policy:
     * The DOI® Kernel Metadata Declaration
     * DOI® Referent Metadata Declaration schemas for data interchange between RAs
     * The Data Dictionary ("DD")
  * https://www.doi.org/VMF/index.html
    * "VMF is a downloadable tool, originally developed with funding from the Joint Information Services Committee (JISC), currently hosted and administered by the International DOI Foundation (IDF) under the guidance of an independent multi-stakeholder Advisory Board. It provides support for semantic interoperability across communities by providing extensive and authoritative mapping of vocabularies from content metadata standards and proprietary schemes."
  * https://www.doi.org/doi_handbook/schemas/dd/intro.html
  * https://www.doi.org/doi_handbook/DataModelUnderlyingOntology.pdf
* Real Estate Standards Organization, Data Dictionary 
  * https://www.reso.org/wp-content/uploads/2016/11/RESO-DD-OWL-Fall-Conference-reduced_Chime.pdf
    * "Introduce a knowledge representation technology (Ontology Web Language) to the Data Dictionary to prevent misunderstanding in communication and ensure semantic interoperability"
  * https://www.reso.org/data-dictionary/#download
* Adobe Experience Manager (v6.4) - Data Dictionary Feature
  * https://helpx.adobe.com/experience-manager/6-4/forms/using/data-dictionary.html
  * https://helpx.adobe.com/experience-manager/6-4/forms/using/data-dictionary.html#DDValidations
* Financial Industry Business Ontology (FIBO) 
  * https://spec.edmcouncil.org/fibo/
  * https://spec.edmcouncil.org/fibo/fibopedia/master/latest/FIBOpedia.html
  * https://spec.edmcouncil.org/fibo/doc/FIBO_Primer.pdf
    * "Industry standard resource for the definitions of business concepts in the financial services industry"
    * "developed and hosted by the Enterprise Data Management Council (EDMC)"
    * "developed as a series of ontologies in the Web Ontology Language (OWL)... it is not a data model but a representation of the “things in the world” of financial services."
    * "ensures that each real-world concept is framed in a way that is unambiguous and that is readable both by humans and machines."
    * FIBO Product:
      * FiboPedia - Annotated structure of FIBO ontologies and modules
      * Glossary  - Human-readable, cross-referenced dictionary of terms in FIBO (in HTML, .csv and Excel™)
      * Data Dictionary  – Am Excel spreadsheet of FIBO terms in .csv and Excel™. Included is an unabridged version, i.e. 100% of FIBO. CAUTION – contains much unvetted material
      * FIBO-Vocabulary  - A machine-readable taxonomy of terms in FIBO (in extended SKOS)
      * SMIF - Machine- and human-readable UML diagrams of FIBO (using the forthcoming OMG UML profile “SMIF”) Semantic Modeling for Information Federation)
      * VOWL (Visual OWL) - Generated web documentation for each ontology, including graphical depictions of FIBO concepts (using the VOWL notation)
      * Ontology Files  – Machine-readable files in the Web Ontology Language (OWL), in a variety of different formats
      * Linked Data Fragments – A way of searching for a particular FIBO Triple, or executing a query 
      * Ontology Files  – Machine-readable files in the Web Ontology Language (OWL), in a variety of different formats
      * schema.org - A vocabulary for marking up web pages for search engines, which has been extended with terms taken from FIBO



### Open Source Tools
* http://jena.apache.org/
  * "A free and open source Java framework for building Semantic Web and Linked Data applications."
* https://marmotta.apache.org/
  * Apache Marmotta is an Open Platform for Linked Data.
  * "The goal of Apache Marmotta is to provide an open implementation of a Linked Data Platform that can be used, extended and deployed easily by organizations who want to publish Linked Data or build custom applications on Linked Data"
  * Features:    
    * Read-Write Linked Data server for the Java EE stack
    * Pluggable RDF triple stores based on Eclipse RDF4J (formerly Sesame):
      * Custom triple store (KiWi) built on top of RDBMS, with transactions, versioning and rule-base reasoning support
      * And some other backends
    * LDP, SPARQL and LDPath querying
    * Transparent Linked Data Caching
    * Integrated basic security mechanisms
  * https://github.com/nicholsn/docker-marmotta
* https://github.com/nicholsn/rdflib
  * RDFLib is a Python library for working with RDF, a simple yet powerful language for representing information. 
  * https://rdflib.readthedocs.io/en/stable/
* https://www.semantic-mediawiki.org/wiki/Semantic_MediaWiki
  * "Semantic MediaWiki is also a full-fledged frame­work, in con­junc­tion with many spin­off ex­ten­sions, that can turn a wiki into a pow­er­ful and flex­i­ble know­ledge manage­ment sys­tem. All data cre­ated with­in Semantic MediaWiki can easi­ly be ex­port­ed or pub­lish­ed via the Semantic Web, al­low­ing other sys­tems to use this data seam­less­ly."
* https://github.com/opensemanticsearch/solr-ontology-tagger
  * "Automatic tagging and analysis of documents in an Apache Solr index for faceted search by RDF(S) Ontologies & SKOS thesauri"
  * https://opensemanticsearch.org/solr-ontology-tagger
  * https://github.com/opensemanticsearch
  * https://opensemanticsearch.org/graph-explorer
    * Look at the visualization/graph example...
    * Integrates Python Django, Apache Solr and Cytoscape.js
    * "The open source tool Open Semantic Visual Linked Data Knowledge Graph Explorer is a web app providing user interfaces (UI) to discover, explore and visualize linked data in a graph for visualization and exploration of direct and indirect connections between entities like people, organizations and locations in your Linked Data Knowledge Graph (for example extracted from your documents by Open Semantic Search or Open Semantic ETL using Named Entity Extraction and Named Entity Recognition)."
* Mobi
  * https://mobi.inovexcorp.com/
  * "Collaborate on data models to increase interoperability."
  * "The Mobi Solution Platform links all your data into an enterprise model, and provides the tools and APIs that empower your team to build better solutions."
  * https://mobi.inovexcorp.com/features/
* NASA CFS Command and Data Dictionary Tool (CCDDT) 
  * https://github.com/nasa/CCDD 
* BEDES-Manager
  * https://github.com/Maalka/BEDES-Manager
  * "A project to ease the management of the management of terms in the Building Energy Data Exchange Standard dictionary."
* https://github.com/tetherless-world/SemanticDataDictionary
  * Tools and specifications for Semantic Data Dictionaries 
* https://github.com/scossin/IAMsystem
  * "IAMsystem, a general purpose biomedical semantic annotation tool. It's a dictionary-based approach with typos and abbreviations detection. The dictionary is stored in a tree data-structure." 
* http://www.dotnetrdf.org/
  * https://github.com/dotnetrdf/dotnetrdf
  * An Open Source .NET Library for RDF
  * A powerful and flexible API for working with RDF and SPARQL 
  * A complete library for parsing, managing, querying and writing RDF.
  * A common .NET API for working with RDF triple stores such as AllegroGraph, Jena, Stardog and Virtuoso.
  * A suite of command-line and GUI tools for working with RDF under Windows
  * MIT License
* https://protege.stanford.edu/
  * "A free, open-source ontology editor and framework for building intelligent systems"
  * "Protégé’s plug-in architecture can be adapted to build both simple and complex ontology-based applications. Developers can integrate the output of Protégé with rule systems or other problem solvers to construct a wide range of intelligent systems."
  * "Protégé fully supports the latest OWL 2 Web Ontology Language and RDF specifications from the World Wide Web Consortium. "
  * https://protege.stanford.edu/support.php#documentationSupport
  * https://github.com/protegeproject/webprotege
* RDF Pro
  * http://rdfpro.fbk.eu/
  * "RDFpro (RDF Processor) is a public domain, Java command line tool and library for RDF processing. RDFpro offers a suite of stream-oriented, highly optimized RDF processors for commo    n tasks that can be assembled in complex pipelines to efficiently process RDF data in one or more passes. RDFpro originated from the need of a tool supporting typical Linked Data integration tasks, involving dataset sizes up to few billions triples."



### Other List of Tools (may not be "fresh")
* http://www.mkbergman.com/sweet-tools/
  * HUGE list...
* http://semanticweb.org/wiki/Tools.html
  * last updated 2012...
* https://opensemanticsearch.org/graph-explorer



### Commercial Tools
* [Data Access Group, MetaCenter](https://www.dag.com/)
  * "Collaborate on data models to increase interoperability."
* [RDF Studio, LinkedDataTools.com](http://www.linkeddatatools.com/rdf-studio)
* http://www.cognitum.eu/semantics/FluentEditor/
  * "Edit your ontologies easier, faster and smarter!"
  * Note: "Fluent Editor is free for individual developers, open source projects, academic research, education, and small professional teams."
  * W3C Standards Supported: OWL 2, OWL-DL, OWL-RL, SWRL, SPARQL, RDF, OCNL
* TopBraid Composer 
  * https://www.topquadrant.com/tools/modeling-topbraid-composer-standard-edition/
* RDF Pro
  * http://rdfpro.fbk.eu/
  * "RDFpro (RDF Processor) is a public domain, Java command line tool and library for RDF processing. RDFpro offers a suite of stream-oriented, highly optimized RDF processors for common tasks that can be assembled in complex pipelines to efficiently process RDF data in one or more passes. RDFpro originated from the need of a tool supporting typical Linked Data integration tasks, involving dataset sizes up to few billions triples."



### GraphDB Tools 
* https://www.ontotext.com/products/graphdb/




### Articles
* 2018 
  * [Data Dictionary: a how to and best practices, Carl AndersonDirector of Data Science, Weight Watchers, NYC. Author of "Creating a Data-Driven Organization" (2015, O'Reilly). Web: carlanderson.ai](https://medium.com/@leapingllamas/data-dictionary-a-how-to-and-best-practices-a09a685dcd61)
* 2016
  * [Using OWL for the Real Estate Standards Organization (RESO) Data Dictionary](https://www.reso.org/wp-content/uploads/2016/11/RESO-DD-OWL-Fall-Conference-reduced_Chime.pdf)
* 2006  
  * [Data Modeling, RDF, & OWL – Part One: An Introduction To Ontologies](http://tdan.com/data-modeling-rdf-owl-part-one-an-introduction-to-ontologies/5025)
* ????
  * [Relational.OWL - A Data and Schema Representation Format Based on OWL, Institute of Computer Science
Heinrich-Heine-Universit ̈at D ̈usseldor](http://crpit.com/confpapers/CRPITV43deLaborda.pdf?q=relational)



### Suggested Books
* [Semantic Web for the Working Ontologist: Effective Modeling in RDFS and OWL, 2nd Edition](https://www.amazon.com/Semantic-Web-Working-Ontologist-Effective-ebook/dp/B005508PX4/)



### Tutorials
* [RDFS vs OWL](https://www.cambridgesemantics.com/blog/semantic-university/learn-owl-rdfs/rdfs-vs-owl/)
* [Tutorial 3: Semantic Modeling](http://www.linkeddatatools.com/semantic-modeling)
* [Tutorial 4: Introducing RDFS & OWL](http://www.linkeddatatools.com/introducing-rdfs-owl)
* [RDF & OWL: A simple overview of the building blocks of the Semantic Web](https://www.slideshare.net/rlovinger/rdf-and-owl)
* [Data Modeling, RDF, & OWL – Part One: An Introduction To Ontologies, by David Hay, TDAN.com April 2006](http://tdan.com/data-modeling-rdf-owl-part-one-an-introduction-to-ontologies/5025)


### Footnotes
[1] [2002, Justice Standard XML Data Dictionary - Justice Information Sharing](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=15&cad=rja&uact=8&ved=2ahUKEwje-4P956zeAhUGBHwKHXCOBSY4ChAWMAR6BAgGEAI&url=https%3A%2F%2Fit.ojp.gov%2FNISS%2FDownloads%2FIEPD%2F152&usg=AOvVaw2F8GxwJQHzl6TmFtoSVluU)
