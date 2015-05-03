[![Build Status](https://travis-ci.org/concordion/concordion-run-totals-extension.svg?branch=master)](https://travis-ci.org/concordion/concordion-logging-tooltip-extension)

This [Concordion](http://www.concordion.org) extension adds run totals to the Concordion output whenever the concordion:run annotation is used.


# Introduction

This extension allows us to reveal run totals in the Concordion output, without obscuring the intent of the specification. For example:

![Logging Tooltip Image](images/RunTotalsOutput.png)



# Installation

This extension requires concordion 1.5.0 (yet to be released)

# Configuration

## Default Configuration


To install the extension, either annotate the fixture class with:

```java
    @Extensions(RunTotalsExtension.class)
```

or set the system property `concordion.extensions` to `org.concordion.ext.runtotals.RunTotalsExtension`.
