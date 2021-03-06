# EDA Skill Journey

Implementing cloud native, event-driven solution with microservices deployed on kubernetes involves a broad skill set. We are proposing here a learning journey for developer with good programming background. This project includes best practices and basic knowledge on the technologies. 

The reference implementation [in this project](https://ibm-cloud-architecture.github.io/refarch-kc) includes a set of technologies we are using that represent the modern landscape of cloud native applications (Kafka, maven, java, microprofile, spring boot, python, nodejs, and postgresql) but also some specific analytics and AI components like Streams analytics and machine learning with Jupyter notebook. A developer who wants to consume this content does not need to know everything at the expert level. You can progress by steps and it will take a good month to digest everything. We are also proposing a bootcamp to build, deploy and re-implement part of the ["Reefer container shipment solution"](https://ibm-cloud-architecture.github.io/refarch-kc). We expect you have some base knowledge on the following technologies.

* Nodejs / Javascript / Typescripts
* Java 1.8 amd microprofile architecture
* Python 3.6
* Angular 7, HTML, CSS
* Maven, npm, bash
* WebSphere Liberty or OpenLiberty
* Docker
* Docker compose
* Helm
* Kubernetes
* Apache Kafka, Kafka API


## Technology getting started

From the list above, the following getting started and tutorials can be studied to get a good pre-requisite knowledge:

* [From zero to hero in Java 1.8](https://www.infoworld.com/article/3130466/java/java-8-programming-for-beginners-go-from-zero-to-hero.html)
* [Liberty getting started application](https://github.com/IBM-Cloud/get-started-java)
* [Getting started with Apache Maven](https://maven.apache.org/what-is-maven.html)
* [Getting started Nodejs and npm](https://nodejs.org/en/docs/guides/getting-started-guide/)
* [Getting started with Apache Kafka](https://kafka.apache.org/quickstart) and [Confluent blog for getting started](https://www.confluent.io/blog/apache-kafka-getting-started/)
* [Angular tutorial](https://angular.io/tutorial)
* [Docker getting started](https://docs.docker.com/get-started/)
* [Getting started with Open Liberty](https://openliberty.io/guides/getting-started.html)
* [Kubernetes](https://kubernetes.io/docs/tutorials/kubernetes-basics/) and IBM developer [learning path for Kubernetes](https://developer.ibm.com/series/kubernetes-learning-path/) and the Garage course [Kubernetes 101](https://www.ibm.com/cloud/garage/content/course/kubernetes-101/0).

* [Use the "Develop a Kubernetes app with Helm" toolchain](https://www.ibm.com/cloud/garage/tutorials/use-develop-kubernetes-app-with-helm-toolchain)
* [Getting started in Python](https://www.python.org/about/gettingstarted/)

## Event Driven Specifics

Now the event driven microservice involve specific technologies and practice. The following links should be studied in the proposed order:

* [Why EDA now?](https://www.ibm.com/cloud/garage/architectures/eventDrivenArchitecture)
* EDA fundamentals:
    * [Reference architecture](https://www.ibm.com/cloud/garage/architectures/eventDrivenArchitecture/reference-architecture)
    * [Event sources](https://www.ibm.com/cloud/garage/architectures/eventDrivenArchitecture/event-driven-event-sources)
    * [Event backbone](https://www.ibm.com/cloud/garage/architectures/eventDrivenArchitecture/event-driven-event-backbone)
    * [Act after an event with IBM Cloud Functions](https://www.ibm.com/cloud/garage/architectures/eventDrivenArchitecture/event-driven-take-action-with-cloud-functions)
    * [Processing continuous streaming events](https://www.ibm.com/cloud/garage/architectures/eventDrivenArchitecture/event-driven-event-streams)
    * [Event-driven cloud-native applications](https://www.ibm.com/cloud/garage/architectures/eventDrivenArchitecture/event-driven-cloud-native-apps)
* Methodology to understand how to jumpstart an event-driven solution with the business team: 
    * [Event storming methodology](https://www.ibm.com/cloud/garage/architectures/eventDrivenArchitecture/event-storming-methodology)
    * [A concrete example to apply event storming, for a container shipment use case.](https://ibm-cloud-architecture.github.io/refarch-kc/analysis/readme/)

## Kubernetes, docker, microprofile, kafka

* As we can use docker compose to control the dependencies between microservices and run all the solution as docker containers, it is important to read the [Docker compose - getting started](https://docs.docker.com/compose/gettingstarted/) article. 
* Kafka is [Getting started with IBM Cloud Event Streams](https://cloud.ibm.com/docs/services/EventStreams?topic=eventstreams-getting_started#getting_started) the IBM product based on Kafka on public cloud
* [IBM Cloud Private Event Streams](https://www.ibm.com/cloud/event-streams) the IBM product based on Kafka for private cloud
* [Understand docker networking](https://docs.docker.com/network/) as we use docker compose to run the reference implementation locally. 
* [The evolving hybrid integration reference architecture](https://developer.ibm.com/articles/mw-1606-clark-trs/): How to ensure your integration landscape keeps pace with digital transformation
* [Deploy MicroProfile-based Java microservices on Kubernetes](https://developer.ibm.com/patterns/deploy-microprofile-java-microservices-on-kubernetes/)

# Virtual bootcamp

The next steps beyond getting started can be done as a set of related labs in a one week timeframe. The source of the bootcamp is the ["Reefer container shipment solution"](https://ibm-cloud-architecture.github.io/refarch-kc).

* [The solution introduction](https://ibm-cloud-architecture.github.io/refarch-kc/introduction)
* [If not already done review the Reefer container shipment use case and event storming analysis](https://ibm-cloud-architecture.github.io/refarch-kc/analysis/readme/)
* [Prepare the solution dependencies](https://ibm-cloud-architecture.github.io/refarch-kc/local): In this first lab we are going from cloning the main repository to prepare all the services and components.
* Get a local Kafka backbone environment up and running to facilitate your development and testing. [Get an event backbone up and running on your laptop in less than 3 minutes](https://ibm-cloud-architecture.github.io/refarch-kc/deployments/local/#start-kafka-and-zookeeper).

* [How to deploy, manage, and secure your container-based workloads on IKS](https://www.ibm.com/blogs/bluemix/2017/05/kubernetes-and-bluemix-container-based-workloads-part1/) and [part 2](https://www.ibm.com/blogs/bluemix/2017/05/kubernetes-and-bluemix-container-based-workloads-part2/)
* [Our Kubernetes troubleshooting notes](https://github.com/ibm-cloud-architecture/refarch-integration/blob/master/docs/icp/troubleshooting.md)
* [Applying a test driven practice for angular application](https://github.com/ibm-cloud-architecture/refarch-caseportal-app/blob/master/docs/tdd.md)
* [Java microprofile application](https://microprofile.io/)
* [Our Cloud Architecture team's bluecompute solution: Microprofile based Microservice Apps Integration with MySQL Database Server](https://github.com/ibm-cloud-architecture/refarch-cloudnative-micro-orders/tree/microprofile)
* [Kafka API consumer](http://kafka.apache.org/11/javadoc/index.html?org/apache/kafka/clients/consumer/KafkaConsumer.html) with our [own summary and implementation considerations](./kafka/consumers.md)
* [Kafka API producer](http://kafka.apache.org/11/javadoc/index.html?org/apache/kafka/clients/producer/KafkaProducer.html) ith our [own summary and implementation considerations](./kafka/producers.md)
* [Kafka Stream APIs](https://kafka.apache.org/documentation/streams/), Java or Scala based API to implement functional processing as a chain of operation to consumer events and generating new event stream. 
* [IBM Cloud Streaming Analytics introduction](https://cloud.ibm.com/catalog/services/streaming-analytics) and [getting started](https://cloud.ibm.com/docs/services/StreamingAnalytics?topic=StreamingAnalytics-gettingstarted#gettingstarted)

### KC Solution labs

* [Deploying the solution locally](https://ibm-cloud-architecture.github.io/refarch-kc/deployments/local/)
* [Deploying the solution on IBM Cloud Kubernetes Service](https://ibm-cloud-architecture.github.io/refarch-kc/deployments/iks)


### Event Driven Specifics

* [Extended Reference Architecture](https://www.ibm.com/cloud/garage/architectures/eventDrivenExtendedArchitecture) with machine learning workbench and event sourcing as data source, and real time analytics for deployment.
* [Event driven design pattern for microservice](./evt-microservices/ED-patterns.md) 
* [IBM Event Streams - National Oceanic and Atmospheric Administration (NOAA) stream analytics app](https://developer.ibm.com/streamsdev/docs/detect-events-with-streams/) Event detection on continuous feed using Streaming Analytics in IBM Cloud. 
* [Kafka monitoring](./kafka/monitoring.md)
* [Kafka Python API](https://github.com/confluentinc/confluent-kafka-python) and some examples in our [integration tests project](https://ibm-cloud-architecture.github.io/refarch-kc/itg-tests/)
* [Kafka Nodejs API]
* [Knative introduction](https://developer.ibm.com/articles/knative-what-is-it-why-you-should-care/)

## More advanced subjects

* [Kafka HA and enterprise deployment](./kafka/readme.md)
* [End to end reference implementation of EDA solution](https://ibm-cloud-architecture.github.io/refarch-kc). A concrete end to end solution to illustrate the different event-driven patterns. 
* [Mirror maker to maintain replicas cross clusters](https://cwiki.apache.org/confluence/pages/viewpage.action?pageId=27846330)
* [Integrate Kadka with MQ](https://ibm.github.io/event-streams/connecting/mq/)


