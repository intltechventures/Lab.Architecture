
ElasticSearch Resources
====

### References
* https://www.elastic.co/
* https://www.elastic.co/guide/index.html
* https://www.elastic.co/guide/en/logstash/current/index.html
* https://www.elastic.co/guide/en/elasticsearch/reference/current/index.html

### Principles
* https://12factor.net/logs


### Tutorials
* Elastic Youtube Channel
  * https://www.youtube.com/user/elasticsearch/videos
  * [Getting Stared series, 7 videos](https://www.youtube.com/watch?v=MNkdXSzt96E&list=PLhLSfisesZIv16xhlT9VsS2BcqhQkT_n-)

* elastic.co
  * [Log Analytics with Elastic Stack](https://www.elastic.co/videos/logstash-analytics-with-elastic-stack)
  * [Getting Started with Logstash](https://www.elastic.co/guide/en/logstash/current/getting-started-with-logstash.html)
  * [Using Elasticsearch for Log Search and Analysis](https://www.elastic.co/webinars/using-elasticsearch-for-log-search-and-analysis)
  * [Getting Started with the Elastic Stack on Microsoft Azure, (2017)](https://www.elastic.co/blog/getting-started-with-elasticsearch-and-the-elastic-stack-on-microsoft-azure)
  * [Deploying Elasticsearch on Microsoft Azure, (2017)](https://www.elastic.co/blog/deploying-elasticsearch-on-microsoft-azure)
    * "Elasticsearch - Data Nodes We found the DS series of memory optimized instances to be a good fit. Like every other data store Elasticsearch is very dependent on the amount of memory available to itself (as the JVM heap) and to the underlying host system (used for the important filesystem cache). You can read a bit more about how memory should be assigned in this blog post."
    * "We also recommend using Premium Storage. Backed by Solid State Drives (SSD) it allows Elasticsearch to reach its stored data quickly - and users will benefit from improved response times. Premium Managed Disks also come with encryption at rest (via Storage Service Encryption)."
    * "Elasticsearch - Master Nodes For bigger clusters, we recommend having three dedicated master nodes. They will not be storing any data, but will handle cluster management tasks like creating new indices and rebalancing shards. Small D series instances are most often good enough."
    * "Kibana Same as master nodes, Kibana has relatively light resource requirements. Most computations are pushed down to Elasticsearch, so you can usually run Kibana on small D series instances as well."
    * "Logstash Since it typically does a lot of processing it is best deployed on the FS series."
  * [Elasticsearch and Kibana Deployments on Azure](https://www.elastic.co/blog/elasticsearch-and-kibana-deployments-on-azure)
  * [Spinning up a cluster with Elastic's Azure Marketplace template, (2016)](https://www.elastic.co/blog/spinning-up-a-cluster-with-elastics-azure-marketplace-template]

* Sematext Youtube Channel
  * [Log Analysis with Elasticsearch, part 1](https://www.youtube.com/watch?v=dkauUMimEgc)
  * [Log Analysis with Elasticsearch, part 2](https://www.youtube.com/watch?v=lv8gJgPx2cQ)

* AWS
  * https://aws.amazon.com/getting-started/projects/build-log-analytics-solution/

* Digital Ocean 
  * [How To Install Elasticsearch, Logstash, and Kibana (Elastic Stack) on Ubuntu 16.04](https://www.digitalocean.com/community/tutorials/how-to-install-elasticsearch-logstash-and-kibana-elastic-stack-on-ubuntu-16-04)
    * " We will install all of these components ```on a single server```, which we will refer to as our Elastic Stack server."

* Kubernetes.io 
  * [Logging Using Elasticsearch and Kibana](https://kubernetes.io/docs/tasks/debug-application-cluster/logging-elasticsearch-kibana/)

* Logz.io
  * https://logz.io/blog/
  * https://logz.io/learn/complete-guide-elk-stack/
  * https://logz.io/learn/docker-monitoring-elk-stack/
  * https://logz.io/blog/the-cost-of-doing-elk-stack-on-your-own/
  * [How to Deploy the ELK Stack in Production](https://logz.io/blog/deploy-elk-production/)
  * [How to Install the ELK Stack on Azure](https://logz.io/blog/install-elk-stack-azure/)



### Slideshare decks
* 2017
  * https://www.slideshare.net/AmazonWebServices/deep-dive-on-log-analytics-with-elasticsearch-service
* 2012
  * https://www.slideshare.net/dadoonet/ElasticSearch-devoxx-france-2012-english-version
  * https://www.slideshare.net/kucrafal/scaling-massive-elastic-search-clusters-rafa-ku-sematext



### Articles
* 2018
  * [Dzone,Data Analytics on Application Events and Logs Using Elasticsearch, Logstash, and Kibana](https://dzone.com/articles/running-data-analytics-on-application-events-and-l)
  * [Our Experience of Creating Large Scale Log Search System Using ElasticSearch](https://www.cubrid.org/blog/our-experience-creating-large-scale-log-search-system-using-elasticsearch)
  * [Getting started on Elasticsearch + Logstash + Kibana + Filebeat (for Nginx logs analysis](https://medium.com/@saurabhpresent/getting-started-on-elasticsearch-logstash-kibana-filebeat-for-nginx-logs-analysis-d567999d7846)
  * [Elastic Stack — A Brief Introduction](https://hackernoon.com/elastic-stack-a-brief-introduction-794bc7ff7d4f)
  * [Best of 2018: Log Monitoring and Analysis: Comparing ELK, Splunk and Graylog](https://devops.com/log-monitoring-and-analysis-comparing-elk-splunk-and-graylog/)
  * [ELK Adventures Part 1](https://medium.com/@Joachim8675309/elk-adventures-part-1-99de2a234423)
    * Related: [Vagrant: Dynamic Multi-Machines](https://medium.com/@Joachim8675309/vagrant-dynamic-multi-machines-1aaad3e64c96)
  * [ElasticSearch, LogStash and Kibana (ELK) on Azure App Services](http://lukieb.blogspot.com/2018/01/elasticsearch-logstash-and-kibana-elk.html)


* 2017
  * [https://www.loggly.com/resource/elk-total-cost-ownership-handbook](https://www.loggly.com/resource/elk-total-cost-ownership-handbook/)
  * [Infographic: The real costs of ELK (Elastic Stack) Log Management ](https://www.loggly.com/blog/elkonomics-real-costs-of-elastic-stack/)
    * Interesting points about cost growth...
      * "a business with average daily log volumes growing from 100 GB to 800 GB over a four-year period will likely spend close to $4.2 million to operate and maintain a production-grade Elastic Stack."
  * [How to Use Elasticsearch, Logstash, and Kibana to Manage Logs](https://qbox.io/blog/how-to-elasticsearch-logstash-kibana-manage-logs)
  * [Research on Establish an Efficient Log Analysis System with Kafka and Elastic Search](https://www.scirp.org/Journal/PaperInformation.aspx?PaperID=79974)
  * [(Designing the Perfect Elasticsearch Cluster: the (almost) Definitive Guide](https://thoughts.t37.net/designing-the-perfect-elasticsearch-cluster-the-almost-definitive-guide-e614eabc1a87)
  * [Splunk and the ELK Stack: A Side-by-Side Comparison](https://devops.com/splunk-elk-stack-side-side-comparison/)


* 2015
  * [DZone, Presentation: Log Analysis with Elasticsearch](https://dzone.com/articles/presentation-log-analysis-with-elasticsearch-1)
  * [Centralized Logging with ELK Stack (Elasticsearch, Logstash, and Kibana) On Ubuntu 14.04 ](https://www.digitalocean.com/community/tutorial_series/centralized-logging-with-elk-stack-elasticsearch-logstash-and-kibana-on-ubuntu-14-04)
  * [How To Use Kibana Dashboards and Visualizations](https://www.digitalocean.com/community/tutorials/how-to-use-kibana-dashboards-and-visualizations)



### Github Resources
* AWS
  * https://github.com/aws-samples/amazon-cloudfront-log-analysis/tree/master/lab2-elk-cloudfront-log-analysis
* Azure
  * https://github.com/Azure/azure-quickstart-templates/tree/master/elasticsearch
    * https://www.elastic.co/blog/azure-cloud-plugin-for-elasticsearch
* Elastic, re: Azure Marketplace
  * https://github.com/elastic/azure-marketplace
    * https://azuremarketplace.microsoft.com/en-us/marketplace/apps/elastic.elasticsearch/


