
# APM Assessment Resources

- I have seen organizations waste hundreds of thousands of dollars in useless
exerecises to attempt to assess applications for Technical and Busienss fit.

- Those exercises inevitably devolve into the business stakeholders discarding the
carefully collected metrics - and dictating to Enterprise Architects where to
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

  + Let the x-axis represent the plot for Business Fit.

  + Let the y-axis represent the plot for the Technical fit.

  + Let the range for the x and y axis be integer values in the range of 0-10. 

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


