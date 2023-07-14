# A Java/Maven/JUnit HelloWorld example

![example branch parameter](https://github.com/mevijays/java-action/actions/workflows/codeql-check.yaml/badge.svg)

![example branch parameter](https://github.com/mevijays/java-action/actions/workflows/mvn-build.yaml/badge.svg)      ![GitHub top language](https://img.shields.io/github/languages/top/mevijays/java-action)



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

