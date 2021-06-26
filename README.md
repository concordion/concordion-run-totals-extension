[![Build and Test](https://github.com/concordion/concordion-run-totals-extension/actions/workflows/ci.yml/badge.svg)](https://github.com/concordion/concordion-run-totals-extension/actions/workflows/ci.yml)
[![Maven Central](https://img.shields.io/maven-central/v/org.concordion/concordion-run-totals-extension.svg)](http://search.maven.org/#search%7Cga%7C1%7Cg%3A%22org.concordion%22%20AND%20a%3A%22concordion-run-totals-extension%22)
[![Apache License 2.0](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](http://www.apache.org/licenses/LICENSE-2.0.html)

This [Concordion](http://www.concordion.org) extension adds run totals to the Concordion output whenever the [concordion:run](https://concordion.org/Tutorial.html#concordion:run) command is used.

# Introduction

This extension allows us to reveal run totals in the Concordion output, without obscuring the intent of the specification. For example:

![Run Totals Output Image](images/RunTotalsOutput.png)

# Installation
The extension is available from [Maven Central](http://search.maven.org/#search%7Cga%7C1%7Cg%3A%22org.concordion%22%20AND%20a%3A%22concordion-run-totals-extension%22).

### Dependencies
Due to breaking API changes in Concordion, you will need to ensure the correct version is in use dependent on your Concordion version:

| `concordion` version | `concordion-run-totals-extension` version |
| ------------------   | ---------------------- |
| <  1.5.0             | n/a                    |
| >= 1.5.0 and < 2.1.0 | 1.0.0                  |
| >= 2.1.0 and < 2.2.0 | 1.1.0                  |
| >= 2.2.0             | 1.2.0                  |

# Configuration

## Default Configuration

To install the extension, either annotate the fixture class with:

```java
    @Extensions(RunTotalsExtension.class)
```

or set the system property `concordion.extensions` to `org.concordion.ext.runtotals.RunTotalsExtension`.
