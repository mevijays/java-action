# A Java/Maven/JUnit HelloWorld example

![example branch parameter](https://github.com/mevijays/java-action/actions/workflows/codeql-check.yaml/badge.svg)

![example branch parameter](https://github.com/mevijays/java-action/actions/workflows/mvn-build.yaml/badge.svg)

[![Quality Gate Status](https://sonarqube.k8s.mevijay.dev/api/project_badges/measure?project=my-custom-project&metric=alert_status&token=72471a9c2ae97875761c86a7b371e3edd0d2384c)](https://sonarqube.k8s.mevijay.dev/dashboard?id=my-custom-project)
[![Coverage](https://sonarqube.k8s.mevijay.dev/api/project_badges/measure?project=my-custom-project&metric=coverage&token=72471a9c2ae97875761c86a7b371e3edd0d2384c)](https://sonarqube.k8s.mevijay.dev/dashboard?id=my-custom-project)
[![Code Smells](https://sonarqube.k8s.mevijay.dev/api/project_badges/measure?project=my-custom-project&metric=code_smells&token=72471a9c2ae97875761c86a7b371e3edd0d2384c)](https://sonarqube.k8s.mevijay.dev/dashboard?id=my-custom-project)
[![Vulnerabilities](https://sonarqube.k8s.mevijay.dev/api/project_badges/measure?project=my-custom-project&metric=vulnerabilities&token=72471a9c2ae97875761c86a7b371e3edd0d2384c)](https://sonarqube.k8s.mevijay.dev/dashboard?id=my-custom-project)
A „Hello World!” sample written in Java using Maven for the build, that showcases a few very simple tests.

This example demonstrates:

* A simple Java 1111111111111111111111 application with tests
* Unit tests written with [JUnit 5](https://junit.org/junit5/)
* Integration tests written with [JUnit 5](https://junit.org/junit5/)
* Code coverage reports via [JaCoCo](https://www.jacoco.org/jacoco/)
* A Maven build that puts it all together

## Running the tests

* To run the unit tests, call `mvn test`
* To run the integration tests as well, call `mvn verify`
* Code coverage reports are generated when `mvn verify` (or a full `mvn clean install`) is called.
  Point a browser at the output in `target/site/jacoco-both/index.html` to see the report.

## Conventions

This example follows the following basic conventions:

| | unit test | integration test |
| --- | --- | --- |
| **resides in:** | `src/test/java/*Test.java` | `src/test/java/*IT.java` |
| **executes in Maven phase:** | test | verify |
| **handled by Maven plugin:** | [surefire](http://maven.apache.org/surefire/maven-surefire-plugin/) | [failsafe](http://maven.apache.org/surefire/maven-failsafe-plugin/) |
ghh
