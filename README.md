# Biggyani OS (BOS)

**Biggyani OS** is a Linux-based operating system project focused on developing a stable, modular, secure, and extensible general-purpose operating system with its own desktop environment.

The project begins with Debian GNU/Linux as its foundation and KDE Plasma as its initial desktop environment. Its long-term objective is to progressively develop independent Biggyani system components and the **Biggyani Desktop Environment (BDE)**.

## Project Vision

To develop an independently identifiable, maintainable, and accessible operating system built on established Linux technologies, with a progressive path toward its own desktop environment and system ecosystem.

## Current Foundation

| Area | Technology |
|---|---|
| Base system | Debian GNU/Linux |
| Kernel | Linux |
| Initial desktop | KDE Plasma |
| Programming languages | C, C++, Python |
| Compiler | GCC / G++ |
| Build system | CMake |
| Build tool | Ninja |
| Version control | Git |
| Initial development platform | VirtualBox |

Technology choices may evolve as the project develops.

## Development Objectives

- Build a bootable BOS prototype.
- Make BOS installable in VirtualBox.
- Establish the Biggyani visual identity.
- Customize and integrate KDE Plasma.
- Validate basic system functionality and offline operation.
- Develop independent Biggyani system utilities.
- Progressively develop the Biggyani Desktop Environment (BDE).
- Establish reproducible packaging and distribution procedures.

## Repository Structure

```text
Biggyani-OS/
├── assets/       # Branding and visual assets
├── config/       # BOS configuration
├── docs/         # Project documentation
├── packaging/    # Packaging and distribution
├── profiles/     # System profiles
├── scripts/      # Development and build scripts
├── src/
│   ├── desktop/  # Desktop components
│   ├── installer/# Installation components
│   ├── system/   # System components
│   └── utilities/# BOS utilities
├── tests/        # Testing and validation
├── .gitignore
└── README.md
```

## Documentation

| Document | Description |
|---|---|
| [System Architecture](docs/architecture.md) | BOS architecture, components, and technical direction |
| [Development Roadmap](docs/development-roadmap.md) | Development phases, milestones, and objectives |

## Development Status

**Current stage:** Development foundation.

The development environment and initial repository structure have been established. Architecture and roadmap documentation are being prepared.

The immediate milestone is to produce a bootable and installable BOS prototype based on Debian.

## Future Direction

- **BDE:** Biggyani Desktop Environment — the long-term independent desktop environment.
- **BROS:** Biggyani Researcher OS — a future research-oriented environment built on the BOS foundation.
- **Kolpona:** A separate future VR/AR and Digital Twin environment.

BROS and Kolpona are outside the current BOS development scope.

## Development Philosophy

BOS follows an incremental development approach:

- Stability before experimentation.
- Modularity and maintainability.
- Offline-first essential functionality.
- Hardware compatibility.
- Security and reliability.
- Open-source technologies wherever practical.
- Progressive independence from existing desktop components.

---

**Project:** Biggyani OS  
**Abbreviation:** BOS  
**Status:** Under active development.
