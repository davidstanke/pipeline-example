# pipeline-example
A simple repo to run multistep pipeline CI against

## TODO
* Create a Jenkins pipeline with 3(+) steps:
    * Validate -- "mvn validate" (will run checkstyle)
    * Test -- "mvn test" (will compile and test, and includes errorprone)
    * Package -- "mvn package" (will build a JAR)

_(the latter steps each re-runs the previous steps, because that's easiest to config; it's redundant but it allows us to fail the build at each of the steps)_
