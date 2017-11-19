#### distributionLocation

##### Usage

Mandatory

##### Type

free text

##### Definition/Explanations

Any location \(e.g. URL, repository, etc.\) where the resource can be accessed from, either in a downloadable form or as a web executable command etc.

**Recommended usage**

* For components registered through Maven, use the Maven coordinates preceded by "mvn:", e.g. `<distributionLocation>mvn:de.tudarmstadt.ukp.dkpro.core:de.tudarmstadt.ukp.dkpro.core.berkeleyparser-gpl:1.9.0-SNAPSHOT#de.tudarmstadt.ukp.dkpro.core.berkeleyparser.BerkeleyParser</distributionLocation>`
* For components registered as Docker images, use the name under which they are registered in the Docker Central hub, e.g. `<distributionLocation>bibliome/alvisengine</distributionLocation>`
* For web services, use the URL endpoint where it can be invoked from
* Worfklows created in the OpenMinTeD platform, are automatically assigned the relevant value.

##### Relation to other metadata schemas

* **Maven POM 4.0.0:** can be done through ID



