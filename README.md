# Java-hello-world-with-gradle

##### This guide walks you through using Gradle to build a simple Java project.

### What you’ll need
+ A favorite text editor or IDE
+ A Java Development Kit (JDK), version 8 or higher - for example [AdoptOpenJDK](https://adoptopenjdk.net/)
+ Install [Gradle](https://gradle.org/install)

### Create a project folder

Gradle comes with a built-in task, called `init`, that initializes a new Gradle project in an empty folder. 
The init task uses the (also built-in) `wrapper` task to create a Gradle wrapper script, `gradlew`.

The first step is to create a folder for the new project and change directory into it.
```
$ mkdir Demo
$ cd Demo
```

### Run the init task
From inside the new project directory, run the `init` task using the following command in a terminal:
`gradle init`. When prompted, select the 2: `application` project type and 3: `Java` as implementation
language. Next you can choose the DSL for writing buildscripts - 1 : `Groovy` or 2: `Kotlin`. For the other 
questions, press enter to use the default values.

The output will look like this:
```
$ gradle init

Select type of project to generate:
  1: basic
  2: application
  3: library
  4: Gradle plugin
Enter selection (default: basic) [1..4] 2

Select implementation language:
  1: C++
  2: Groovy
  3: Java
  4: Kotlin
  5: Scala
  6: Swift
Enter selection (default: Java) [1..6] 3

Select build script DSL:
  1: Groovy
  2: Kotlin
Enter selection (default: Groovy) [1..2] 1

Select test framework:
  1: JUnit 4
  2: TestNG
  3: Spock
  4: JUnit Jupiter
Enter selection (default: JUnit 4) [1..4] 4

Project name (default: demo):
Source package (default: demo):


BUILD SUCCESSFUL
2 actionable tasks: 2 executed
```

## Run the application


```
$ ./gradlew run

```

## Bundle the application
```
$ ./gradlew build

```
## Publish a build scan

```
$ ./gradlew build --scan

BUILD SUCCESSFUL in 0s
7 actionable tasks: 7 executed

Publishing a build scan to scans.gradle.com requires accepting the Gradle Terms of Service defined at https://gradle.com/terms-of-service.
Do you accept these terms? [yes, no] yes

Gradle Terms of Service accepted.
Publishing build scan...
https://gradle.com/s/2suich5xjmziu
```
Here is my [link](https://gradle.com/s/2suich5xjmziu) for my built scan

##Summary
That’s it! You’ve now successfully configured and built a Java application project with Gradle. You’ve learned how to:

Initialize a project that produces a Java application

Run the build and view the test report

Execute a Java application using the `run` task from the `application` plugin

Bundle the application in an archive



