# Spring Data JPA Kickstart Project

This project provides basic skeleton setup for a Spring Data MongoDB based app. It will set up the following:

* A plain Java project based on the latest Spring Data MongoDB release and Logback for logging.
* The necessary Spring XML configuration (`src/main/resources/META-INF/spring/application-context.xml`) to set up 
** `Mongo` and `MongoDbFactory` instances for connecting to the Mongo Server. 
** `MongoTemplate` and `GridFsTemplate` 
** Activate Spring Data repository support
* A mongodb.properties file containing host and port properties to connect to the MongoDB Server
* A sample `ApplicationTest` (in `com.acme` inside `src/test/java`) to bootstrap this configuration.

To adapt the skeleton to your needs you mostly need to do the following:

* Adapt groupId and artifactId according to your project requirements
* Change the host and port parameters in mongodb.properties based on your environment
* Create entities and repositories inside `src/main/java` according to your project and adapt the `base-package` attribute in the `<mongo:repositories />` element inside `src/main/resources/META_INF/spring/application-context.xml` 
