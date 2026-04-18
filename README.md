# EmbeddedX

🧭 **You are here (canonical index).**

## Specifications for Structured Embedded Development

**Canonical entry point:** this `EmbeddedX-Specs` repository is the umbrella index for the full EmbeddedX specification family.

Proposed by: Richard Haberkern  
Contact: rmhaberkern@gmail.com

Free for evaluation. Commercial use requires permission. See [LICENSE.md](./LICENSE.md) for more information.

* * *

## Abstract

Embedded development still depends on information scattered across datasheets, schematics, netlists, board files, SDK examples, application notes, and local project rules.

That works for experienced engineers, but it creates problems for repeatable development and controlled code generation. Tools need to know which files are inputs, which files are generated outputs, what can be modified, and what must remain unchanged.

EmbeddedX defines a set of related specifications for hardware data, board connectivity, reusable development kit inputs, model metadata, runtime integration, code generation controls, and deployable packages.

EmbeddedX is not a replacement for existing development environments, vendor documentation, SDKs, or engineering review. It is a family of specifications and workspace conventions that other tools and repositories can build on.

* * *

## 1. Core Specification Family

The platform currently centers on:

* **Machine Readable Datasheet (MRD)** - hardware capability and constraint definition
* **Machine Readable Connectivity (MRC)** - board connectivity definition
* **Standardized Developer Package (SDP)** - reusable vendor and board input package
* **Model Definition Package (MDP)** - model interface and behavior definition
* **Embedded Intelligence Layer (EIL)** - bounded runtime intelligence layer
* **AI Integrated Coding System (AICS)** - controlled integration and code generation system
* **Embedded Intelligence Package (EIP)** - deployment and package structure

* * *

## 2. Recommended Reading Order

1. `EmbeddedX-Specs/README.md` (this page)
2. **SDP** (how reusable board/vendor inputs are organized)
3. **MRD** (device capability/constraints firmware can rely on)
4. **MRC** (what is connected on the actual board)
5. **MDP** (model interface + runtime assumptions)
6. **EIL** (bounded integration into firmware)
7. **AICS** (controlled generation + validation + restore points)
8. **EIP** (deployable packaging)

* * *

## 3. Objective

EmbeddedX aims to reduce setup churn, integration mistakes, and undocumented assumptions in embedded projects.

The specification family is intended to support systems that can:

* describe hardware in machine-readable form
* describe real board connectivity in machine-readable form
* organize reusable vendor and board inputs
* describe embedded models in a portable and structured form
* integrate runtime intelligence through clear boundaries
* generate and modify code using constrained workflows
* preserve human visibility, editability, validation, rollback, and recovery
* standardize reusable developer inputs across vendors, boards, and components

* * *

## 4. Repository Structure

This umbrella repository defines the shared structure. The sibling specification repos fill in the technical details:

* **Machine Readable Datasheet (MRD)** defines hardware capabilities and constraints
* **Machine Readable Connectivity (MRC)** defines board connectivity facts
* **Standardized Developer Package (SDP)** organizes reusable vendor and board inputs
* **Model Definition Package (MDP)** defines model interfaces and behavior
* **Embedded Intelligence Layer (EIL)** defines runtime boundaries
* **AI Integrated Coding System (AICS)** defines coding, validation, and recovery controls
* **Embedded Intelligence Package (EIP)** defines deployable package structure

Together, these specs give generation and validation tools a concrete input surface before they touch firmware.

* * *

## 5. Project Framework

EmbeddedX also defines how a user creates and manages a project.

The project framework includes:

* shared library structure
* project workspace structure
* required project files
* required portable project memory
* agent roles
* rules and control boundaries
* state management and restore points
* vendor and development kit organization
* Standardized Developer Package (SDP) input rules

* * *

## 6. Simplified File Tree

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
      /memory
```

Full project and library tree: [docs/full-file-tree.md](docs/full-file-tree.md)

* * *

## 7. Key Framework Documents

* [docs/project-framework.md](docs/project-framework.md)
* [docs/portable-project-memory.md](docs/portable-project-memory.md)
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

## 8. Specification Repositories

* [Machine-Readable-Datasheets-Specs](https://github.com/telespial/Machine-Readable-Datasheets-Specs)
* [Machine-Readable-Connectivity-Specs](https://github.com/telespial/Machine-Readable-Connectivity-Specs)
* [Standardized-Developer-Package-Specs](https://github.com/telespial/Standardized-Developer-Package-Specs)
* [Model-Definition-Package-Specs](https://github.com/telespial/Model-Definition-Package-Specs)
* [Embedded-Intelligence-Layer-Specs](https://github.com/telespial/Embedded-Intelligence-Layer-Specs)
* [AI-Coding-System-Specs](https://github.com/telespial/AI-Coding-System-Specs)
* [Embedded-Intelligence-Package-Specs](https://github.com/telespial/Embedded-Intelligence-Package-Specs)

* * *

## License

See [LICENSE.md](./LICENSE.md) for terms.
