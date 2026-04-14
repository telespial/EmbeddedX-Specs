# EmbeddedX Library Structure

## Overview

The EmbeddedX shared library contains reusable assets across vendors, boards, components, specifications, Software Development Kit environments, debug flows, and sample code.

The library exists so projects do not duplicate information that should be reusable.

## High-Level Structure

```text
/library
  /vendors
  /components
  /specs
  /sdk
  /debug
```

## Component Classes

Reusable components should be organized by class, for example:

* MCU
* MPU
* Sensors
* Displays
* Wireless
* Power
* Storage
* Audio
* Connectors
* Logic
* Passives
* Protection
* Timing
* Other
