# EmbeddedX Development Kit Structure

## Overview

Development kits should be treated as first-class reusable library assets. They are not just board names or example folders. They are structured board objects with documentation, sample code, SDK references, debug references, and board-specific specification links.

## Development Kit Folder Pattern

```text
/library/vendors/<vendor>/boards/<board_name>/
  board.manifest.json
  start_here.md
  /docs
  /schematics
  /netlists
  /bom
  /sample_code
  /sdk_refs
  /debug_refs
  /specs
    /mrd
    /mrc
  /notes
```
