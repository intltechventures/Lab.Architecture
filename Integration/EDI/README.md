 
# Electronic Data Interchange (EDI) Integration 


## My EDI Experience 

- I first began exploring EDI back in the early 1990s, when I formed Ozark Information Services, as my first professional consulting business. 

- I attended an early CORBA/EDI conference in Seattle (1992?), where I met [Eric Schmidt](https://en.wikipedia.org/wiki/Eric_Schmidt)

- 1999-2001, while working as the Development Manager for a [Paul Allen](https://en.wikipedia.org/wiki/Paul_Allen) e-commerce ventura (Mercata, Inc.; funded by his [Vulcan Ventures, Inc.](https://en.wikipedia.org/wiki/Vulcan_Real_Estate)), I implemented EDI interfaces with a number of the company's white-label suppliers.

- 2020-2022, during an Enterprise Architecture consulting engagement with a healthcare payer firm in Seattle, I helped advise Solution Architects on the design of integration solutions that levereaged healthcare EDI transactions.


## Glossary of Terms

|Term       | Definition|
|-----------|--------------|
5010        | In Electronic Data Interchange (EDI), 5010 (specifically ASC X12 Version 5010) is the standardized format mandated by the Health Insurance Portability and Accountability Act (HIPAA) for transmitting electronic healthcare transactions.
8020        | A newer X12 version, intended to support FHIR and other technologies
ANSI        | American National Standards Institute
ASC         | Accredited Standards Committee 
CAHs        | Critical Access Hospitals
CDC         | Center for Disease Control 
CDT         | Code on Dental Procedures and Nomenclature
CHIP        | Children’s Health Insurance Program
CICA        | Context Inspired Component Architecture
CPT         | Current Procedural Terminology
DEL         | Data Element Library 
EDI         | Electronic data interchange 
EDIFACT     | Electronic Data Interchange for Administration, Commerce, and Transport. A globally recognized UN standard that provides a common syntax and structure for businesses to electronically exchange documents (such as invoices, purchase orders, and shipping notices) across different computer systems, industries, and international borders.
FFEs        | Federally Facilitated Exchanges
FFS         | Fee-for-Service
FHIR        | Fast Healthcare Interoperability Resources
HCPCS       | Healthcare Common Procedure Coding System
HL7         | Health Level 7
ICD-10      | International Classification of Diseases, 10th Revision; the global diagnostic coding system published by the World Health Organization.
ICD-10-CM   | Clinical Modification; Used across all healthcare settings to code patient diagnoses, illnesses, and injuries.
ICD-10-PCS  | Procedure Coding System; Used exclusively in hospital inpatient settings to code medical procedures.
ICD-11      | International Classification of Diseases, 11th Revision
MA          | Medicare Advantage
MIPS        | Merit-based Incentive Payment System
NCHS        | National Center for Health Statistics
NCPDP       | National Council for Prescription Drug Programs
QHP         | Qualified Health Plan
STU         | Standard for Trial Use
UN/CEFACT   | United Nations Centre for Trade Facilitation and Electronic Business 
USCDI       | United States Core Data for Interoperability 
WHO         | World Health Organization
WHO-FIC     | WHO Family of International Classifications


## References

- https://en.wikipedia.org/wiki/Electronic_data_interchange


## EDI Message Standard: EDIFACT

- EDIFACT
  + https://en.wikipedia.org/wiki/EDIFACT
  + https://unece.org/uncefact/unedifact/2021-2024
  + https://www.edibasics.com/edi-resources/document-standards/edifact/
  + https://datainterchange.com/edifacts-standards-explained/



## EDI Message Standard: ANSI ASC x12

- ANSI ASC X12
  + https://en.wikipedia.org/wiki/ASC_X12
    * ASC X12 has sponsored more than 300 X12 EDI transaction sets and a growing collection of X12 XML schemas for health care, insurance, government, transportation, finance, and many other industries
  + https://en.wikipedia.org/wiki/X12_Document_List
  + https://www.edibasics.com/edi-resources/document-standards/ansi/



## EDI Message Exploration Utilities & Tools

- https://edination.edifabric.com
  + https://edination.edifabric.com/edi-spec-library.html



- DFDL Schemas for Commercial and Scientific Data Formats
  + https://dfdlschemas.github.io/
  + https://github.com/DFDLSchemas
    * https://github.com/DFDLSchemas/EDIFACT/
      * United Nations Rules for Electronic Data Interchange for Administration, Commerce and Transport (UN/EDIFACT)
      * This GitHub repository holds DFDL schemas that model UN/EDIFACT interchanges (ISO 9735).


### Technical

- EDI Transmission Mechanisms:
  + SFTP
  + AS2
  + HTTPS


### International Classification of Diseases (ICD)

- https://www.who.int/classifications/classification-of-diseases

- https://icd10cmtool.cdc.gov/


- ICD-10 Codes
  + https://en.wikipedia.org/wiki/ICD-10    
    * Work on ICD-10 began in 1983
    * Endorsed by the Forty-third World Health Assembly in 1990, and came into effect in member states on January 1, 1993
    * ICD-10 was replaced by ICD-11 on January 1, 2022
  + ICD-10-CM codes are alphanumeric and range from 3 to 7
  + Structure: 
    * **Characters 1-3**: Category of the disease or injury.
    * **Characters 4–6**: Details regarding etiology, anatomic site, severity, or related manifestations.
    * **Character  7**: Added for specific encounters (e.g., initial encounter, subsequent encounter, or sequela)
  + Example:
    * ```Code S52.521A``` represents a displaced torus fracture of the lower end of the right radius, initial encounter for a closed fracture.
  + Code Definitons:
    * https://www.icd10data.com/
    * https://www.cms.gov/medicare/coding-billing/icd-10-codes
    * https://www.cdc.gov/nchs/icd/icd-10-cm/index.html


- ICD-11 Codes
  + https://en.wikipedia.org/wiki/ICD-11
    * The ICD-11 is the eleventh revision of the International Classification of Diseases (ICD). It replaces the ICD-10 as the global standard for recording health information and causes of death. The ICD is developed and annually updated by the World Health Organization (WHO). Development of the ICD-11 started in 2007[1][2] and spanned over a decade of work, involving over 300 specialists from 55 countries divided into 30 work groups,[7][8] with an additional 10,000 proposals from people all over the world.[9] Following an alpha version in May 2011 and a beta draft in May 2012, a stable version of the ICD-11 was released on 18 June 2018,
    * The ICD-11 is a large ontology consisting of about 85,000 entities, also called classes or nodes. An entity can be anything that is relevant to health care. It usually represents a disease or a pathogen, but it can also be an isolated symptom or (developmental) anomaly of the body. There are also classes for reasons for contact with health services, social circumstances of the patient, and external causes of injury or death. The ICD-11 is part of the WHO-FIC, a family of medical classifications.
    * Officially endorsed by all WHO members during the 72nd World Health Assembly on 28 May 2019.


### Standards, Compliance, Regulatory

- Seven (7) Elements of an Effective Compliance Program
  + As proscribed by the Federal Sentencing Guidelines issued by the United States Sentencing Commission and the Health and Human Services (HHS) division of the Office of the Inspector General (OIG)
  + Elements:
    * Policies, Procedures, and Controls 
    * Oversight 
    * Performance of Due Diligence 
    * Communication and Education
    * Internal Monitoring and Auditing
    * Enforcement and Discipline 
    * Response to Incidents 


- HIPAA Privacy Program
  + Health Insurance Portability and Accountability Act of 1996 ("HIPAA").
  + Summary of the HIPAA Privacy Rule  
    * https://www.hhs.gov/hipaa/for-professionals/privacy/laws-regulations/index.html


- CMS Adopted Standards and Operating Rules:
  + https://www.cms.gov/priorities/key-initiatives/burden-reduction/administrative-simplification/hipaa/adopted-standards-operating-rules
    * https://www.govinfo.gov/content/pkg/FR-2009-01-16/pdf/E9-740.pdf


- **CMS-0057-F**: Centers for Medicare & Medicaid Services Interoperability & Prior Authorization Final Rule
  + https://www.cms.gov/newsroom/fact-sheets/cms-interoperability-prior-authorization-final-rule-cms-0057-f


- **CMS 85 FR 25510**: May 2020 CMS Interoperability and Patient Access final rule 


- Anti-Bribery and Anti-Corruption (ABAC/FCPA) Compliance Program


- General Data Protection Program


- National Center for Health Statistics  
  + https://www.cdc.gov/nchs/


- World Health Organization 
  + https://en.wikipedia.org/wiki/World_Health_Organization
  + https://www.who.int/ 
  + WHO Family of International Classifications
    * https://en.wikipedia.org/wiki/Medical_classification#WHO_Family_of_International_Classifications


## EDI Transaction Types

- https://en.wikipedia.org/wiki/X12_Document_List



## Retail & Procurement (Supply Chain)

- **X12 850 Purchase Order**: 
  + Buyer's official order initiating a transaction.


- **X12 855 Purchase Order Acknowledgment**: 
  + Supplier's confirmation to accept, reject, or modify the PO.
  + Reduces costly errors by catching discrepancies early while providing transparency and building trust between trading partners.


- **X12 846 Inventory Inquiry**: 
  + Real-time request or communication of stock availability.


- **X12 810 Invoice**: 
  + Supplier's request for payment.


- **X12 875/876 Grocery Products**: 
  + Specialized Purchase Order and Purchase Order Change for the grocery industry



## Logistics & Transportation

- **X12 204 Motor Carrier Load Tender**: 
  + Shipper's request to a carrier to move a load.


- **X12 853 Routing and Carrier Instructions**: 
  + Reduces delivery delays and errors by standardizing transportation details and helps manage compliance with retailer-specific shipping requirements.


- **X12 856 Advance Ship Notice (ASN)**: 
  + Detailed packing and shipping data sent prior to delivery.
  + Allows receiving teams to prepare for incoming shipments, speeding up unloading and inventory updates. ASNs also improve visibility into supply chain events and can help avoid errors and delays.


- **X12 210 Motor Carrier Freight Details**: 
  + Carrier's invoice for transportation services.


- **X12 214 Transportation Carrier Shipment Status**: 
  + Real-time updates on delivery status.


- **X12 940 Warehouse Shipping Order**: 
  + Instruction to a warehouse to ship goods to a customer.
  + Automates communication with third-party warehouses which reduces manual processes and minimizes shipping errors by clearly specifying fulfillment requirements.


- **X12 943 Warehouse Stock Transfer Shipment Advice**:
  + Notifies the receiving warehouse that inventory is on its way during a transfer between locations. Ensures accurate inventory reconciliation by tracking stock transfers and supports multi-location inventory strategies for scalability and distribution.


- **X12 944 Warehouse Stock Transfer Receipt Advice**:
  + The 944 validates inventory accuracy post-transfer, which prevents discrepancies and enhances inventory control by resolving shortage or overage issues immediately.


- **X12 945 Warehouse Shipping Advice**:
  + Confirms the warehouse has shipped the requested goods while providing critical shipment details such as quantities, tracking numbers, and carriers. The 944 also helps reconcile shipments with ASNs (856) and invoices (810) and can reduce disputes by serving as proof of shipment.  



## Finance & Payments

- **X12 820 Payment Order/Remittance Advice**: Details the payment amount and the invoices being paid.


- **X12 812 Credit/Debit Adjustment**: Notification of a financial adjustment between partners.



## Healthcare (HIPAA compliant)

### HIPAA EDI Error Codes

- **X12 999**

- **X12 277CA**



### Insurance Eligibility & Benefits

- **X12 270 Eligibility Inquiry**: 
  + Checking a patient's Eligibility, Coverage or Benefit Inquiry


- **X12 217 Eligibility Response**: 
  + Eligibility, Coverage or Benefit Information


- **X12 834 Benefit Enrollment and Maintenance**: 



### Prior Authorization

- **X12 278 Healthcare Services Review**: 
  + Prior authorization or certification requests.



###  Claim Submission & Validation

- **X12 837 Healthcare Claim**: 
  + Submission of medical claims to insurance payers.


- **X12 835 Healthcare Claim Payment**: 
  + Payer's explanation of benefits (EOB) and payment details.



### Claim Status 

- **X12 276 Claims Status Request**: 
  + Inquiry (EDI 276): The provider asks the payer about the status of a previously submitted claim.


- **X12 277 Claims Status Response**: 
  + Response (EDI 277): The payer updates the provider on whether the claim is in-process, pending further documentation, or rejected.




### Payment & Remittance

- **X12 835 Remittance Advice**: 
  + The payer sends the Electronic Remittance Advice (ERA) to the provider, detailing which services were paid, adjustments, and denials.


- **X12 820 Electronic Funds Transfer (EFT)**: 
  + The payment is transferred directly into the provider's bank account.



## Misc. 

- **X12 816 Organization Relationship**:
  + This document type communicates organizational relationships between headquarters, branches, and warehouses. It lets trading partners share location information including addresses and site codes. It's valuable because keeping trading partners updated about location changes (e.g., new warehouses and closed stores), helps ensure accurate routing and billing.


- **X12 824 Application Advice**:
  + his document type provides feedback about errors or acceptance of an EDI transaction by identifying specific issues or confirmations. It impacts the bottom line by pinpointing issues quickly and reducing processing delays.


- **X12 864 Text Message**:
  + Not a text message in the mobile phone sense, but unstructured text rather than the pre-defined fields of other document types. It communicates freeform messages like explanations, warnings, or special instructions. Users can receive it via email or dashboard alerts within the EDI system.




## System Control

- **X12 997 Functional Acknowledgment**: Confirms that an EDI document was successfully received and checked for syntax errors.


- **X12 999 Implementation Acknowledgement**: 
  + The EDI 999 Implementation Acknowledgement document is used in healthcare to provide confirmation that a file was received. It is similar to the broader X12 EDI 997 FA, however, the 999 gives additional information about potential errors in the received transaction.
  + The EDI 999 transaction set can specifically be used to describe the control structures for a set of acknowledgments to show the results of the syntactical and relational analysis of the documents encoded electronically. The encoded documents are the transaction sets, put together in functional groups that define transactions for business data interchange. 
  + The 999 Acknowledgement gives the following results:
    * Accepted (A)
    * Rejected (R)
    * Accepted with errors (E)



## EDI Vendor Solutions (illustrative, not exhaustive)

- Caveat Emptor: No recommendation is implied, or intended. 



## EDI Clearinghouses & Trading Partner Networks


### Healthcare

- Availity  
  + https://www.availity.com/clearinghouse-and-trading-partner-network/
    * "The Availity Clearinghouse Solution provides national‑scale transaction connectivity and processing across eligibility, authorization, claims, payments, and related administrative workflows—delivered through a single, trusted network, so trading partners can connect once and exchange consistently, while clearinghouse operations run with predictable throughput and controls."
  + https://www.availity.com/blog/
  + https://www.availity.com/training-and-education/
  + https://payernetworkstatus.availity.com/
  + https://www.availity.com/existing-integrations/
  + Payer Lists:
    + https://essentials.availity.com/static/public/onb/onboarding-ui-apps/payer-list-ui/#/  
    + https://essentials.availity.com/static/public/onb/onboarding-ui-apps/payer-list-ui/#/EssentialsPro

  + https://www.glassdoor.com/Overview/Working-at-Availity-EI_IE249487.11,19.htm
    * https://www.glassdoor.com/Reviews/Availity-Reviews-E249487.htm



## EDI Solution Providers, General 

- Epicore
  + https://www.epicor.com/en-us/products/electronic-data-interchange-edi/


- Orderful
 + https://www.orderful.com/
   * "Orderful is a unified EDI platform built to support teams of every size, from small businesses using Web EDI to global enterprises standardizing on an API-powered workflow. Connect once, automate your transactions, and trade with thousands of partners through a modern, scalable network."


- SPS Commerce 
  + https://www.spscommerce.com/


- TrueCommerce
  + https://www.truecommerce.com/
