# EmbeddedX Vendor Hubs

## Overview

Vendor hubs provide structured entry points for reusable vendor-specific assets. They should organize development environments, debugging, examples, boards, and documentation without forcing every project to rediscover the same information.

## Priority Vendor Hubs

The primary MCU and MPU vendor hubs currently expected are:

* Infineon
* Microchip
* NXP
* STMicroelectronics

## Vendor Hub Pattern

```text
/library/vendors/<vendor>/
  vendor.manifest.json
  /sdk
  /debug
  /hal
  /examples
  /boards
  /components
  /docs
```
