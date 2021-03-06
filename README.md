Simple example integrating the commercetools JVM SDK with Spring MVC and Spring DI

<img width="1252" alt="screen shot 2015-12-02 at 10 18 06" src="https://cloud.githubusercontent.com/assets/1320833/11526944/3606ac4a-98de-11e5-8f84-30d700fd6bfe.png">

Create a project
----------------
requirements:
* install [Java 8](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
* install [Maven 2+](https://maven.apache.org)


```bash
mvn archetype:generate \
  -DarchetypeGroupId=com.commercetools.maven-archetypes \
  -DarchetypeArtifactId=commercetools-spring-mvc-quickstart \
  -DarchetypeVersion=0.4.0 \
  -DgroupId=io.sphere.demo \
  -DartifactId=commercetools-spring-mvc \
  -Dversion=0.1.0-SNAPSHOT \
  -DcommercetoolsProjectKey=YOUR-PROJECT-KEY \
  -DcommercetoolsClientId=YOUR-CLIENT-ID \
  -DcommercetoolsClientSecret=YOUR-CLIENT-SECRET
```

Change to the project folder
----------------------------
```bash
cd commercetools-spring-mvc
```

Run the project
----------------

```bash
mvn tomcat7:run
```

Test on the browser
-------------------

[http://localhost:8080/](http://localhost:8080/)


Creating a new project in Eclipse
----------------------------------

* Import archetype URI by `Import ... > Projects from Git > Clone URI`
* Install the archetype in local repository with `mvn install`
* Go to `Preferences > Maven > Archetypes` and `Add Local Catalog`
* Select the catalog from file (`archetype-catalog.xml`) 
* Create new Maven project and select the archetype (remember so select `Include snapshot archetypes`)

If you have any troubles with installation in Eclipse, you may want to have a look at this issue: #74

Credits
-------

This template is a modified copy of https://github.com/kolorobot/spring-mvc-quickstart-archetype
