# Spring-Boot Command Line Demo

A template for [CLI](https://en.wikipedia.org/wiki/Command-line_interface) applications using Spring Boot

# Goal

Provide a working template for building command line tools that leverage the features of Spring-Boot, and JCommander

# Motivation

CLI tools are very flexible, generally good for prototyping and exploration.

Granted that most CLI tools may start out as simple main() functions.

However, any useful tool will require ever more complex features and configurations.

[Spring Boot](https://projects.spring.io/spring-boot/) makes it easier to create stand-alone Spring based applications  

[Learning resources for Spring](https://spring.io/guides) are not too bad, and Spring Boot comes with its own [set of samples](https://github.com/spring-projects/spring-boot/tree/master/spring-boot-samples).

# Features

This demo goes a few steps beyond [spring-boot-sample-simple](https://github.com/spring-projects/spring-boot/tree/master/spring-boot-samples/spring-boot-sample-simple):

1. Maven configured to pack CLI into a single executable JAR
2. running scripts for Unix and Windows
3. [JCommander](http://jcommander.org/) for parsing line arguments
4. a custom ContextInitializer to inject [YAML properties](http://yaml.org/) into the [Spring Environment](http://docs.spring.io/spring/docs/current/javadoc-api/org/springframework/core/env/Environment.html)
5. a couple of tests which disable the CommandLineRunner

Each feature will be discussed on its own.



