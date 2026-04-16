# EmbeddedX

## Specifications for the EmbeddedX Workflow

Proposed by: Richard Haberkern  
Contact: rmhaberkern@gmail.com

Free for evaluation. Commercial use requires permission. See license.md for more information.

* * *

## Abstract

AI-assisted embedded development still depends too heavily on manual interpretation. Hardware behavior is buried in datasheets, board wiring is split across schematics and netlists, model behavior is described inconsistently, and code generation is often too unconstrained for engineers to trust or maintain.

EmbeddedX defines a set of related specifications for hardware data, board connectivity, model metadata, runtime integration, code-generation controls, and deployable packages.

It is not a single tool, runtime, or IDE. It is a family of specifications and workspace conventions that other tools and repositories can build on.

* * *

## 1. Core Specification Family

The platform currently centers on:

* **Machine Readable Datasheet (MRD)** - hardware capability definition
* **Machine Readable Connectivity (MRC)** - real board connectivity definition
* **Model Definition Package (MDP)** - model interface and behavior definition
* **Embedded Intelligence Layer (EIL)** - safe runtime intelligence layer
* **AI Integrated Coding System (AICS)** - controlled integration and code generation system
* **Embedded Intelligence Package (EIP)** - deployment and package structure

* * *

## 2. Objective

EmbeddedX aims to reduce setup churn, integration mistakes, and undocumented assumptions in embedded projects.

The specification family is intended to support systems that can:

* describe hardware in machine-readable form
* describe real board connectivity in machine-readable form
* describe embedded AI models in a portable and structured form
* integrate runtime intelligence through clear boundaries
* generate and modify code using constrained workflows
* preserve human visibility, editability, validation, rollback, and recovery
* standardize reusable developer inputs across vendors, boards, and components

* * *

## 3. Repository Structure

This umbrella repository defines the shared structure. The sibling specification repos fill in the technical details:

- Machine Readable Datasheet (MRD) defines hardware capabilities and constraints
- Machine Readable Connectivity (MRC) defines board connectivity facts
- Model Definition Package (MDP) defines model interfaces and behavior
- Embedded Intelligence Layer (EIL) defines runtime boundaries
- AI Integrated Coding System (AICS) defines coding, validation, and recovery controls
- Embedded Intelligence Package (EIP) defines deployable package structure

Together, these specs give generation and validation tools a more concrete input surface before they touch firmware.

* * *

## 4. Project Framework

EmbeddedX also defines how a user creates and manages a project.

The project framework includes:

* shared library structure
* project workspace structure
* required project files
* agent roles
* rules and control boundaries
* state management and restore points
* vendor and development kit organization
* Standardized Developer Package (SDP) input rules

* * *

## 5. Simplified File Tree

```text
/embeddedx
  /library
    /vendors
    /components
    /specs
  /projects
    /<project_name>
      start_here.md
      project.manifest.json
      project.rules.md
      /generated
      /validation
      /logs
      /states
```

Full project and library tree: [docs/full-file-tree.md](docs/full-file-tree.md)

* * *

## 6. Key Framework Documents

* [docs/project-framework.md](docs/project-framework.md)
* [docs/system-architecture.md](docs/system-architecture.md)
* [docs/agent-architecture.md](docs/agent-architecture.md)
* [docs/rules-and-control.md](docs/rules-and-control.md)
* [docs/state-management.md](docs/state-management.md)
* [docs/library-structure.md](docs/library-structure.md)
* [docs/vendor-hubs.md](docs/vendor-hubs.md)
* [docs/dev-kit-structure.md](docs/dev-kit-structure.md)
* [docs/sdp-spec.md](docs/sdp-spec.md)
* [docs/full-file-tree.md](docs/full-file-tree.md)

* * *

## 7. Related Repositories

* [Machine-Readable-Datasheets-Specs](https://github.com/telespial/Machine-Readable-Datasheets-Specs)
* [Machine-Readable-Connectivity-Specs](https://github.com/telespial/Machine-Readable-Connectivity-Specs)
* [Model-Definition-Package-Specs](https://github.com/telespial/Model-Definition-Package-Specs)
* [Embedded-Intelligence-Layer-Specs](https://github.com/telespial/Embedded-Intelligence-Layer-Specs)
* [AI-Integrated-Coding-System-Spec](https://github.com/telespial/AI-Integrated-Coding-System-Spec)
* [Embedded-Intelligence-Package-Specs](https://github.com/telespial/Embedded-Intelligence-Package-Specs)

* * *

## License

See `license.md` for terms.
