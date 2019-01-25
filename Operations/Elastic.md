
Elastic Stack Resources
====
(NOTE the ">>>" entires as suggested first-look)

### References
* https://www.elastic.co/
* https://www.elastic.co/guide/index.html
* https://www.elastic.co/guide/en/logstash/current/index.html
* https://www.elastic.co/guide/en/elasticsearch/reference/current/index.html
* https://www.elastic.co/guide/en/elastic-stack-overview/6.5/index.html
  * https://www.elastic.co/guide/en/elasticsearch/reference/6.5/release-notes-6.5.4.html


### Principles
* https://12factor.net/logs


### Docker
* Elastic Docker Images
  * https://hub.docker.com/search/?q=ELK&type=image

  * ">>>" Install Elasticsearch with Docker
    * https://www.elastic.co/guide/en/elasticsearch/reference/current/docker.html
    * https://www.elastic.co/guide/en/elasticsearch/reference/6.5/docker.html
      * ```docker pull docker.elastic.co/elasticsearch/elasticsearch:6.5.4```
      * ```docker run -p 9200:9200 -p 9300:9300 -e "discovery.type=single-node" docker.elastic.co/elasticsearch/elasticsearch:6.5.4```

  * https://www.docker.elastic.co/
    * "At Elastic, we care about Docker. We provide Docker images for all the products in our stack, and we consider them a first-class distribution format. We also host a dedicated Docker Registry to provide the best possible experience and the most reliable service for you."
    * "On this page, you'll find all the resources — docker commands, links to product release notes, documentation and source code — for installing and using the Docker images."

* ">>>" ELastic full install, in one command
  * https://www.elastic.co/blog/a-full-stack-in-one-command
    * "As illustrated above, as well as starting containers for Elasticsearch, Kibana and each of our Beats, we spin up instances of NGINX, Apache2 and MySQL.  These provide interfaces for Metricbeat modules (apache, nginx, mysql) to monitor, as well as generating logs that can be consumed by equivalent modules in Filebeat (apache2, nginx, mysql). Furthermore, with some careful bind-mounting of local filesystem locations, Metricbeat can be used to monitor both the host's system statistics (via the system module) and the Docker containers themselves (via the docker module).  Filebeat can additionally be used to collect and ingest the host's system logs using its equivalent of the system module, as well as the Docker JSON logs generated as a result of the containers sending their output to stdout. We use Packetbeat to collect and monitor any DNS, HTTP, or other layer-7 traffic traffic occurring on the host, including MySQL transaction data. Although not illustrated above (to avoid a spider web of connecting lines), Heartbeat monitors all other containers via ICMP,  performs health checks against Kibana, Elasticsearch, Apache2 and NGINX over HTTP, and against MySQL through a raw TCP socket connection."

  * ">>>" Install Elsatic Stack, running on a single machine
    * https://github.com/elastic/stack-docker
    * The Elastic Stack, on Docker, right now. 
      * "This example Docker Compose configuration demonstrates many components of the Elastic Stack, all running on a single machine under Docker."
      * "At least 4GiB of RAM for the containers. Windows and Mac users must configure their Docker virtual machine to have more than the default 2 GiB of RAM"

  * https://github.com/elastic/kibana-docker
    * https://github.com/elastic/kibana-docker/tree/6.5
    * Official Kibana Docker image 
    * The images have been tested on Docker 17.03.1-ce.

  * ">>>" Popular Docker contributed image for Elastic Search
    * https://hub.docker.com/r/sebp/elk
    * NOTE: Over 5M downloads...
    * This Docker image provides a convenient centralised log server and log management web interface, by packaging Elasticsearch, Logstash, and Kibana, collectively known as ELK.
    * https://github.com/spujadas/elk-docker

* ">>>" ```For Azure```
  * https://www.elastic.co/guide/en/logstash/current/azure-module.html
    * "The Microsoft Azure module in Logstash helps you easily integrate your Azure activity logs and SQL diagnostic logs with the Elastic Stack."
    * "You can monitor your Azure cloud environments and SQL DB deployments with deep operational insights across multiple Azure subscriptions. You can explore the health of your infrastructure in real-time, accelerating root cause analysis and decreasing overall time to resolution."
    * "The Elastic Stack version 6.4 (or later) is required for this module."
    * "Azure Monitor should be configured to stream logs to one or more Event Hubs. Logstash will need to access these Event Hubs instances to consume your Azure logs and metrics."
    * "An Azure Blob Storage account is an essential part of Azure-to-Logstash configuration. It is required for users who want to scale out multiple Logstash instances to consume from Event Hubs."
    * "The instructions below assume that you have Logstash, Elasticsearch, and Kibana running locally. You can also run Logstash, Elasticsearch, and Kibana on separate hosts." 
    * ```As of 2019-01-25, "Warning: This functionality is experimental and may be changed or removed completely in a future release.``` Elastic will take a best effort approach to fix any issues, but experimental features are not subject to the support SLA of official GA features."
    * https://www.elastic.co/guide/en/logstash/6.5/plugins-inputs-azure_event_hubs.html 

  * [Deployment of Kibana+Elasticsearch Containers with Docker Compose](https://github.com/Azure/azure-quickstart-templates/tree/master/docker-kibana-elasticsearch)
    * "This template allows you to deploy an Ubuntu Server 15.04 VM with Docker (using the Docker Extension) and starts a Kibana container listening on port 5601 which uses Elasticsearch database running in a separate but linked Docker container, which are created using Docker Compose capabilities of the Azure Docker Extension."

* ">>>" Examples:
  * https://github.com/elastic/examples
    * "Home for Elasticsearch examples available to everyone. It's a great way to get started."
    * "This is a collection of examples to help you get familiar with the Elastic Stack and X-Pack. Each example folder includes a README with detailed instructions for getting up and running with the particular example. The following information pertains to the examples repo as a whole."

  * https://github.com/elastic/examples/tree/master/Miscellaneous/docker/full_stack_example
    * https://github.com/elastic/examples/tree/master/Miscellaneous/docker/full_stack_example#dashboards-with-data
    * "The following dashboards are accessible and populated. Other dashboards, whilst loaded, will not have data due to the absence of an appropriate container e.g. Packetbeat Cassandra."
      * CPU/Memory per container
      * DNS
      * Filebeat Apache2 Dashboard
      * Filebeat MySQL Dashboard
      * Filebeat Nginx Dashboard
      * Filebeat syslog dashboard - Not available on Windows
      * Heartbeat HTTP monitoring
      * Metricbeat - Apache HTTPD server status
      * Metricbeat Docker
      * Metricbeat MySQL
      * Metricbeat filesystem per Host
      * Metricbeat system overview
      * Metricbeat-cpu
      * Metricbeat-filesystem
      * Metricbeat-memory
      * Metricbeat-network
      * Metricbeat-overview
      * Metricbeat-processes
      * Packetbeat Dashboard (limited)
      * Packetbeat Flows
      * Packetbeat HTTP
      * Packetbeat MySQL performance



### Security Concerns
* Use security best practices to secure your configuration.
  * https://www.elastic.co/guide/en/elastic-stack-overview/6.5/xpack-security.html



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


### White Papers
* https://logdna.com/whitepapers/true-cost-of-elk-stack/


### Articles
* [Monitor ASP.NET Core in ELK through Docker and Azure Event Hubs](https://medium.com/@marcodesanctis2/monitor-asp-net-core-in-elk-through-docker-and-azure-event-hubs-6e519249af61)
* [Deployment of full-scale ELK stack to Kubernetes (on AWS)](https://hackernoon.com/deployment-of-full-scale-elk-stack-to-kubernetes-6f38f6c57c55)
  * https://github.com/ITSvitCo/aws-k8s/tree/master/kubernetes-manifests/elasticsearch/ 
* [Setup ELK for NGINX logs with Elasticsearch, Logstash, and Kibana](https://pawelurbanek.com/elk-nginx-logs-setup)
* [How to Install the ELK Stack on Azure](https://dzone.com/articles/how-to-install-the-elk-stack-on-azure)
* [How much does free ELK stack cost you?](https://coralogix.com/log-analytics-blog/how-much-does-free-elk-stack-cost-you/)
  * "We went for the classic case of a mid-size company:"
    * 50GB of log data per day.
    * Retention period of 14 days.
    * High data availability.
  * "Total estimated price for building your own ELK stack on AWS: 716$ + 110$ + 1590$ = 2416$/month"
  * "Total estimated price for a simple managed ES on AWS with Kibana and Logstash: 1032$ + 574$ = 1606$/month"


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
  * [Start with Elasticssearch, Kibana and ASP.NET Core](https://carlos.mendible.com/2017/05/30/start_with_elasticsearch_kibana_and_aspnet_core/)


* 2015
  * [DZone, Presentation: Log Analysis with Elasticsearch](https://dzone.com/articles/presentation-log-analysis-with-elasticsearch-1)
  * [Centralized Logging with ELK Stack (Elasticsearch, Logstash, and Kibana) On Ubuntu 14.04 ](https://www.digitalocean.com/community/tutorial_series/centralized-logging-with-elk-stack-elasticsearch-logstash-and-kibana-on-ubuntu-14-04)
  * [How To Use Kibana Dashboards and Visualizations](https://www.digitalocean.com/community/tutorials/how-to-use-kibana-dashboards-and-visualizations)


### Videos
* 2017
  * [OpenDev 10.2017 | Logging, security, and analytics on Azure with the Elastic Stack](https://www.youtube.com/watch?v=tOqWX9JWEYc)




### Github Resources
* AWS
  * https://github.com/aws-samples/amazon-cloudfront-log-analysis/tree/master/lab2-elk-cloudfront-log-analysis

* Azure
  * https://github.com/Azure/azure-quickstart-templates/tree/master/elasticsearch
    * https://www.elastic.co/blog/azure-cloud-plugin-for-elasticsearch

* Elastic, re: Azure Marketplace
  * https://github.com/elastic/azure-marketplace
    * https://azuremarketplace.microsoft.com/en-us/marketplace/apps/elastic.elasticsearch/

* Serilog
  * https://github.com/serilog/serilog-sinks-elasticsearch

* https://github.com/stevewillson/elastic_stack_test
  * docker containers and scripts to test elastic stack functionality 




### Bitnami Azure Resources
* Bitnami
  * https://docs.bitnami.com/azure/apps/elasticsearch/
  * https://bitnami.com/stack/elk
    * "The Bitnami ELK Stack provides a one-click install solution for ELK. Download installers and virtual machines, or run your own ELK server in the cloud."
  * https://bitnami.com/stack/elk/cloud/azure 
  * https://docs.bitnami.com/azure/apps/elk/


