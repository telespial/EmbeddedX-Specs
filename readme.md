# EmbeddedX

## A System for Building Embedded Products with Integrated Intelligence

Proposed by: Richard Haberkern  
Contact: rmhaberkern@gmail.com

Free for evaluation. Commercial use requires permission. See license.md for more information.

* * *

## Abstract

Embedded development still depends too heavily on fragmented human interpretation. Hardware behavior is buried in datasheets, board wiring is scattered across schematics and netlists, model behavior is described inconsistently, and AI-assisted code generation is often too unconstrained for engineers to trust, review, and maintain.

EmbeddedX is a platform that defines a structured system for AI-driven embedded development across hardware, connectivity, models, runtime, coding, and deployable packages.

EmbeddedX is not a single tool, runtime, or IDE. It is a platform framework intended to support a family of independent specifications, reusable libraries, controlled project workspaces, and future implementations.

* * *

## 1. Core Specification Family

The platform currently centers on:

* **Machine Readable Datasheet (MRD)**: describes what hardware can do
* **Machine Readable Connectivity (MRC)**: shows how the board is wired using schematics, netlists, BOM files, and board files
* **Model Definition Package (MDP)**: defines model inputs, outputs, and behavior
* **Embedded Intelligence Layer (EIL)**: adds safe runtime intelligence alongside firmware
* **AI Integrated Coding System (AICS)**: controls integration, validation, and code generation
* **Embedded Intelligence Package (EIP)**: packages the deployable output

* * *

## 2. Platform Objective

EmbeddedX aims to reduce risk and development cost while accelerating time to market for embedded products.

The platform is intended to support systems that can:

* describe hardware in machine-readable form
* show how a board is connected using schematics, netlists, BOM files, and board files
* describe embedded AI models in a portable and structured form
* integrate runtime intelligence through clear boundaries
* generate and modify code using constrained workflows
* preserve human visibility, editability, validation, rollback, and recovery
* standardize reusable developer inputs across vendors, boards, and components

* * *

## 3. Framework-First Architecture

EmbeddedX is a framework-first platform.

The umbrella repository defines the platform rules first, then the sibling specifications operate under that framework:

* **Machine Readable Datasheet (MRD)** describes hardware capability
* **Machine Readable Connectivity (MRC)** shows how the schematic, nets, components, and board connections fit together
* **Model Definition Package (MDP)** defines model inputs, outputs, and behavior
* **Embedded Intelligence Layer (EIL)** defines where intelligence can run without changing the firmware control path
* **AI Integrated Coding System (AICS)** controls code generation, validation, and recovery
* **Embedded Intelligence Package (EIP)** defines how deployable outputs are packaged

These layers work together to reduce ambiguity before generated firmware reaches physical hardware.

* * *

## 4. First Project Walkthrough

A first EmbeddedX project should be easy to follow:

1. Choose a vendor and development kit
2. Load the Standardized Developer Package (SDP), if available
3. Link the schematic, netlist, BOM, datasheets, sample code, and board files
4. Link or generate Machine Readable Datasheet (MRD) files
5. Link or generate Machine Readable Connectivity (MRC) files
6. Create `start_here.md`, `project.manifest.json`, and `project.rules.md`
7. Run validation checks before generating code
8. Generate only into approved project folders
9. Promote a validated result to candidate or golden state

This makes the process visible, repeatable, and recoverable.

* * *

## 5. Project Framework

EmbeddedX also establishes how a user creates and manages a project.

The project framework defines:

* shared library structure
* project workspace structure
* required project files
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
```

Full project and library tree: [docs/full-file-tree.md](docs/full-file-tree.md)

* * *

## 7. Key Framework Documents

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
* [docs/market-position.md](docs/market-position.md)

* * *

## 8. Related Repositories

* [Machine-Readable-Datasheets-Specs](https://github.com/telespial/Machine-Readable-Datasheets-Specs)
* [Machine-Readable-Connectivity-Specs](https://github.com/telespial/Machine-Readable-Connectivity-Specs)
* [Model-Definition-Package-Specs](https://github.com/telespial/Model-Definition-Package-Specs)
* [Embedded-Intelligence-Layer-Specs](https://github.com/telespial/Embedded-Intelligence-Layer-Specs)
* [AI-Integrated-Coding-System-Spec](https://github.com/telespial/AI-Integrated-Coding-System-Spec)
* [Embedded-Intelligence-Package-Specs](https://github.com/telespial/Embedded-Intelligence-Package-Specs)

* * *

## License

See `license.md` for terms.
