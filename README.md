# javawc

The `Java Word Count` ia a Java application built with the purpose of showcasing the usage of some Java 8 features, e.g. Streams, Lambdas. 
This application is very similar to Linux 'wc' tool, which basically display some statistics related to one file (number of lines, words, etc).

## Requirements
- Java 8

## Usage
To use this application you need [gradle](http://gradle.org/), but you don't need to download Gradle to start using it. 
This project is configured to use the [Gradle Wrapper](https://docs.gradle.org/current/userguide/gradle_wrapper.html) which is a
Gradle feature which allows a developer to execute the build without having to install Gradle, making your build more reliable.

This project is configured to call the distribution gradle task by default, so, to generate your distribution package which contains all the assets
required to run this application, just open a console pointing to the project root folder and run the command:

```bash
$ ./gradlew
```
Then it will start downloading all the gradle dependencies and after awhile your build should be successful.

For start using `javawc`, you just need to go to folder `/build/install/JavaWC/bin` and then run `./wc <filename>`.

```bash
$ ./wc file.txt
Lines: 16
Words: 16
average letters per word: 5.00
most common letter: l
```

## Generate distribution package (.zip and .tar)
You can find a distribution package in both .zip and .tar format under the `/build/distribution` folder
which contains the source code, documentation, binaries and script files for running this application.

They are organized in the following folders:
- `bin`: script files (.bat or binary)
- `lib`: javawc binaries (.jar & .jar dependencies)
- `src`: source code
- `javadoc`: javadoc


