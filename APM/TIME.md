
# Application Portfolio Management (APM) Assessment Resources


## Introduction

- I have seen organizations waste hundreds of thousands of dollars in useless
exerecises to attempt to assess applications for Technical and Busienss fit - by
attempting to obtain greater and greater information fideltiy - with more and
more paramters. Person-years of effort were expended - and no valuable insights
were obtained.

- The intent is not to conduct a highly accurate data science exercise - the
  intent is to provide a context and framework for the beginning of a discussion on Application Rationalization.

- Those exercises inevitably devolved into the business stakeholders discarding the
carefully collected _subjective metrics_ - and dictating to Enterprise Architects where to
plot the applications in a traditional Gartner TIME quadrant diagram:

  + Tolerate
  + Invest
  + Migrate
  + Elimiate


- Additionally, when you have more than a handfull of metrics to aggregate for the
derivation of either Technical or Business Fit - you will invariably hide the
worst of the lot by summing and averaging a value for the x or y axis plot. 

- Therefore, my recommendation is to simply adopt a subjective, and much simpler,
scoring strategy (since that is where you will end-up anyway).

  + Let the x-axis represent the plot for **Business Fit**.

  + Let the y-axis represent the plot for the **Technical fit**.

  + Let the range for the x and y axis be integer values in the range of **0-10**. 

  + Let the size of a bubble plot correspond to the **Total Annual Costs** for an
    Application (which should include: Licensing Costs, Internal and External
    maintenance/development costs, hosting/infrastructure costs).

  + Let the color of a bubble plot correspond to the **Business Criticality** of an
    Application (as defined by an associated *Recovery Point Objective* and
    *Recovery Time Objective*). The following are suggestive/illustrative only.
    * **Low**
      * RPO: 72 hours
      * RTO: 72 hours
    * **Medium**
      * RPO: 24 hours
      * RTO: 24 hours
    * **High**
      * RPO: 8 hours
      * RTO: 8 hours
    * **Critical**
      * RPO: 1 hour
      * RTO: 1 hour


The following provides some initial guidance for the definition and meeaning of
Busienss and Technical Fit.


## Business Fit (x-axis, 0=Low, 10=High)
The degree to which the application...

- Provides the desired business functionality

- Is easy to use
  + User Interface
  + Accessability
  + Meaningful prompts and error messages
  + Good quality documentation

- Can easily support changing business requirements


## Technical Fit (y-axis, 0=Low, 10=High)
The degree to which the application...

- Aligns with the long-term Enterprise Architecture technical roadmap

- Utilizes underlying technologies which are well maintained and secure

- Conforms with the organization's Enterprise Architecture Principles, Policies,
  Standards, and Specifications

- Provides an appropriate level (based on busienss requirements) of:
  + Scalability
  + Reliability
  + Availability 
  + Performance
  + Security

- Integrates with the organization's operational processes:
  + Monitoring & Observability
  + Logging
  + Alerting 
  + DevOps, Deployment
  + Backup/Recovery


