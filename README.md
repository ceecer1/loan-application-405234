
# Kalix Workshop - Loan application - Java
Not supported by Lightbend in any conceivable way, not open for contributions.
## Prerequisite
Java 11 or later<br>
Apache Maven 3.6 or higher<br>
[Kalix CLI](https://docs.kalix.io/kalix/install-kalix.html) <br>
Docker 20.10.14 or higher (to run locally)<br>
Container registry with public access (like Docker Hub)<br>
Access to the `gcr.io/kalix-public` container registry<br>
cURL<br>
IDE / editor<br>

## Create kickstart maven project

```
mvn archetype:generate \
-DarchetypeGroupId=io.kalix \
-DarchetypeArtifactId=kalix-maven-archetype \
-DarchetypeVersion=1.3.2
```
Define value for property 'groupId': `io.kx`<br>
Define value for property 'artifactId': `loan-application` <br>
Define value for property 'version' 1.0-SNAPSHOT: :<br>
Define value for property 'package' io.kx: : `io.kx.loanapp`<br>

## Run
```
mvn compile
```

## Import generated project in your IDE/editor
<i><b>Delete all generated sample proto files after done</b></i>

## Update main class
In `pom.xml`:
1. In `<mainClass>io.kx.loanapp.Main</mainClass>` replace `io.kx.loanapp.Main` with `io.kx.Main`
2. In `<dockerImage>my-docker-repo/${project.artifactId}</dockerImage>` replace `my-docker-repo` with 'your dockerhub username' during the workshop, you can change to your own later.

## Next, refer to loan-application.md file to develop loan application service (if you need assist)
