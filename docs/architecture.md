# EmbeddedX Architecture

## A Framework-First Architecture for Structured AI-Driven Embedded Development

```text
EmbeddedX Framework / Platform
        ├── MRD
        ├── MDP
        ├── EIL
        ├── AICS
        └── EIP
                 ↓
      Generated / Modified Firmware
                 ↓
          Physical Hardware
```

Generated firmware should be constrained by the combined effect of these layers.
Skipping that structure is where things break.
