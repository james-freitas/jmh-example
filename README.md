# Performance measurement with JMH – Java Microbenchmark Harness

JMH is a tool for measuring Java code performance, primarily focused on
microbenchmarks.

## New project

To create a new project that supports JMH run with maven:

```shell
$ mvn archetype:generate \
          -DinteractiveMode=false \
          -DarchetypeGroupId=org.openjdk.jmh \
          -DarchetypeArtifactId=jmh-java-benchmark-archetype \
          -DgroupId=com.company \
          -DartifactId=jmhTest \
          -Dversion=1.0
```

### Build the benchmarks

Run this Maven command in the root folder of your project:

```shell
mvn clean install
```

### Run the benchmarks

Run this Maven command in the root folder of your project:

```shell
java -jar target/benchmarks.jar
```