# Standardized Developer Package (SDP) Specification

## Overview

A Standardized Developer Package (SDP) is a structured package containing the documentation, board data, and software assets required to begin development on a device or development kit.

The SDP is the preferred standardized input bundle for project bootstrap.

## SDP V1 Structure

```text
<board_or_device>.sdp/
  package.manifest.json
  start_here.md

  /hardware
    /datasheets
    /schematics
    /netlists
    /bom

  /software
    /sample_code
    /drivers
    /examples

  /docs
    /quick_start
    /user_guides
    /notes

  /optional
    /mrd
    /mrc
```

## V1 Adoption Rule

Machine-readable specifications such as Machine Readable Datasheet (MRD) and Machine Readable Connectivity (MRC) should be supported as optional in SDP V1 so vendors can adopt the format quickly.
