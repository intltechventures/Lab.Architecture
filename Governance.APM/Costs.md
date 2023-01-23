
# Governance.APM - Costs Modeling

## The Challenages:
- Frequently, I've seen CFOs/Finance teams in orgs that want to roll-up the time-reporting (e.g. from engineering, operations, support, development costs, project costs, support costs, etc.) to an application (or depending on how your CMDB models - it may also make distinctions between business applications, application services, and technical services - a al ServiceNow's Common Service Data Model - version 2, 3, or 4 - and 5 which I believe is under development...and *may* substantially "break" previous model concepts).
- This can be *very* problematic...
- Finance usually has their own level of abstraction for how they are recording software/applications - and it doesn't usually map to the CDMB level of abstraction...
- EAs *usually* have their own level of abstraction...and it never maps to the Finance teams conceptual model...and *rarely* will map to the level of detail in the CMDB (e.g., see how most organizations choose to model things like SAP in ServiceNow (they often don't define down to the module level (which EAs or SAs need - to be able to elaborate solution designs) - and often just have a single Business Application defined for SAP)...
- PMO / time tracking systems...this becomes even *more* problematic...as delivery team are usually not tracking time spent at the application/service/component level - but at a project level - which may span multiple applications for a given block of time recorded...
- It is a rats-nest of complexity to map/bridge the different levels of abstraction between those different groups - to get a good/reliable "match"


## Possible Meta Model Resources
-  TBM Council (formed by Apptio) has defined a technology business management (and finance) meta-model / taxonomy
  + https://www.tbmcouncil.org/
  + https://www.tbmcouncil.org/learn-tbm/tbm-taxonomy/
    * "The Industry's First Hierarchical Taxonomy of IT Services, Towers, and Cost Sources"
  + https://www.apptio.com/solutions/technology-business-management/

