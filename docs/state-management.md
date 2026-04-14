# EmbeddedX State Management

## Overview

State management is part of the EmbeddedX framework, not just part of AICS.

Projects should maintain explicit restore points so changes remain recoverable and trustable.

## Core States

* Working
* Candidate
* Golden
* Failsafe
* Recovery

## State Rules

* a candidate should not silently become golden
* working should not silently overwrite failsafe
* promotion should be intentional and visible
* rollback should be fast, obvious, and repeatable
