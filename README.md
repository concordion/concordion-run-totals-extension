[![Build Status](https://travis-ci.org/concordion/concordion-run-totals-extension.svg?branch=master)](https://travis-ci.org/concordion/concordion-logging-tooltip-extension)

This [Concordion](http://www.concordion.org) extension adds run totals to the Concordion output whenever the concordion:run annotation is used.


# Introduction

This extension allows us to reveal run totals in the Concordion output, without obscuring the intent of the specification. For example:

![Logging Tooltip Image](images/RunTotalsOutput.png)



# Installation
The extension is available from [Maven Central](http://search.maven.org/#artifactdetails%7Corg.concordion%7Cconcordion-run-totals-extension%7C1.1.2%7Cjar).</a>

# Configuration

## Default Configuration


To install the extension, either annotate the fixture class with:

```java
    @Extensions(RunTotalsExtension.class)
```

or set the system property `concordion.extensions` to `org.concordion.ext.runtotals.RunTotalsExtension`.
