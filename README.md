underscore-java8
================

[![Maven Central](https://img.shields.io/maven-central/v/com.github.javadev/underscore8.svg)](http://search.maven.org/#search%7Cga%7C1%7Cg%3A%22com.github.javadev%22%20AND%20a%3A%22underscore8%22)
[![MIT License](http://img.shields.io/badge/license-MIT-green.svg) ](https://github.com/javadev/underscore-java8/blob/master/LICENSE.txt)
[![Build Status](https://secure.travis-ci.org/javadev/underscore-java8.svg)](https://travis-ci.org/javadev/underscore-java8)
[![Run Status](https://api.shippable.com/projects/5a91f397d03865070011c058/badge?branch=master)](https://app.shippable.com/github/javadev/underscore-java8)
[![codecov](https://codecov.io/gh/javadev/underscore-java8/branch/master/graph/badge.svg)](https://codecov.io/gh/javadev/underscore-java8)
[![Quality Gate](https://sonarcloud.io/api/project_badges/measure?project=javadev_underscore-java8&metric=alert_status)](https://sonarcloud.io/dashboard/index/javadev_underscore-java8)
[![Quality Gate](https://sonarcloud.io/api/project_badges/measure?project=javadev_underscore-java8&metric=sqale_rating)](https://sonarcloud.io/dashboard/index/javadev_underscore-java8)

Requirements
============

Java 1.8 and later.

## Installation

Include the following in your `pom.xml` for Maven:

```
<dependencies>
  <dependency>
    <groupId>com.github.javadev</groupId>
    <artifactId>underscore8</artifactId>
    <version>1.7</version>
  </dependency>
  ...
</dependencies>
```

Gradle:

```groovy
compile 'com.github.javadev:underscore8:1.7'
```

Underscore-java is a java port of [Underscore.js](http://underscorejs.org/).

### Usage

```java
U.chain(/* array | list | set | map | anything based on Iterable interface */)
    .filter(..)
    .map(..)
    ...
    .sortWith()
    .forEach(..);
U.chain(value1, value2, value3)...
U.range(0, 10)...

U.chain(1, 2, 3) // or java.util.Arrays.asList(1, 2, 3) or new Integer[] {1, 2, 3}
    .filter(v -> v > 1)
    // 2, 3
    .map(v -> v + 1)
    // 3, 4
    .sortWith((a, b) -> b.compareTo(a))
    // 4, 3
    .forEach(System.out::println);
    // 4, 3
```

In addition to porting Underscore's functionality, Underscore-java includes matching unit tests.

For docs, license, tests, and downloads, see:
http://javadev.github.io/underscore-java

Thanks to Jeremy Ashkenas and all contributors to Underscore.js.
