# Biggyani OS (BOS) — System Architecture

**Project:** Biggyani OS  
**Abbreviation:** BOS  
**Document:** System Architecture  
**Status:** Initial Architecture — Development Foundation

---

## 1. Overview

Biggyani OS (BOS) is a Linux-based operating system project intended to develop into an independent, general-purpose operating system with its own desktop environment and integrated system components.

The project will initially use established Linux technologies and Debian as its foundation. Over time, Biggyani OS will progressively develop its own identity, tools, interfaces, and desktop components.

The long-term objective is to build a maintainable, modular, secure, accessible, and extensible operating system.

## 2. Core Architectural Philosophy

BOS development will follow these principles:

- **Stability:** Prioritize a reliable operating system over experimental features.
- **Modularity:** Keep system components independently maintainable.
- **Offline-first:** Essential operating system functionality must not depend on continuous internet access.
- **Hardware compatibility:** Support a practical range of existing computer hardware.
- **Security:** Follow sound Linux security practices and maintain controlled system access.
- **Maintainability:** Prefer understandable, documented, and maintainable implementations.
- **Open-source orientation:** Prefer open-source technologies and components wherever practical.
- **Progressive independence:** Replace external desktop components gradually rather than attempting to build everything from scratch.

## 3. Base System

The initial BOS foundation will consist of:

| Component | Initial foundation |
|---|---|
| Operating system base | Debian GNU/Linux |
| Kernel | Linux kernel |
| Package management | Debian package ecosystem |
| Desktop environment | KDE Plasma |
| Boot and installation | Established Linux boot and installation technologies |
| Development language | C and C++ where appropriate |
| Build environment | GCC, CMake, Ninja |
| Version control | Git |

These are initial implementation choices, not permanent limitations on the project's future architecture.

## 4. Desktop Environment Architecture

### 4.1 Initial Desktop

KDE Plasma will serve as the initial desktop environment.

The first stage will focus on:
- Desktop branding and visual identity.
- Themes, icons, wallpapers, and interface configuration.
- Panel and launcher customization.
- System settings and usability.
- Integration with the underlying Debian system.

### 4.2 Biggyani Desktop Environment (BDE)

The long-term objective is to develop the Biggyani Desktop Environment (BDE).

BDE is intended to become an independently developed desktop environment rather than remaining a permanently customized KDE Plasma distribution.

Development will be progressive:

1. Customize KDE Plasma.
2. Develop independent Biggyani desktop utilities.
3. Introduce independent interface components.
4. Replace selected KDE-specific components where practical.
5. Progressively establish BDE as an independent desktop environment.

The project will avoid unnecessary duplication of mature Linux functionality.

## 5. Major System Modules

BOS will follow a modular architecture.

### 5.1 System Core

Responsible for the operating system's fundamental integration and configuration.

Potential responsibilities:
- System configuration.
- Service integration.
- System information.
- Hardware identification.
- System-level utilities.

### 5.2 Installer

Responsible for installing BOS onto physical or virtual hardware.

Initial objective:
- Produce a bootable BOS installation image.
- Support installation inside VirtualBox.
- Establish a repeatable installation process.

### 5.3 Desktop

Responsible for the graphical user experience.

Initial foundation: KDE Plasma.

Long-term direction: Biggyani Desktop Environment (BDE).

### 5.4 Utilities

Responsible for supporting applications and system tools.

Examples of future possibilities:
- System monitoring.
- File and storage utilities.
- Network management tools.
- Software management interfaces.
- System maintenance utilities.

### 5.5 Configuration

Contains BOS-specific configuration templates and settings.

### 5.6 Profiles

Provides a foundation for future system configurations and editions.

### 5.7 Packaging

Contains the infrastructure for integrating BOS components into distributable packages and installation images.

### 5.8 Testing

Contains system validation, installation tests, compatibility checks, and automated tests as they are developed.

## 6. Software Architecture and Development Strategy

BOS will initially rely on established Debian and Linux components.

Custom software will be introduced when it provides a meaningful benefit to the project.

The implementation should:
- Separate custom BOS code from external system components.
- Avoid unnecessary modifications to the underlying Debian system.
- Use documented interfaces and established Linux conventions.
- Keep build and configuration processes reproducible.
- Maintain clear boundaries between independent modules.

## 7. Offline-First Operation

BOS must remain usable without a continuous internet connection.

The normal operating system should not require:
- A Biggyani account.
- Mandatory cloud authentication.
- Continuous internet connectivity.

Internet access may be used for software updates, downloading packages, and optional online services.

Essential local operating system functionality should remain available offline.

## 8. Security and Reliability

Security and reliability will be considered throughout development.

Key priorities:
- Appropriate user and administrator permissions.
- Reliable package management.
- Secure system configuration.
- Controlled system services.
- Proper handling of system updates.
- Testing before introducing major system changes.

## 9. Hardware and Platform Strategy

The initial development target is a VirtualBox virtual machine.

VirtualBox provides a controlled environment for:
- System development.
- Boot testing.
- Installation testing.
- Configuration testing.
- Repeatable experiments.

Physical hardware compatibility will be expanded and tested progressively.

The architecture should avoid unnecessary dependence on one specific computer configuration.

## 10. Future Relationship with Other Biggyani Projects

BOS is the general-purpose operating system foundation.

Two separate future projects are envisioned:

- **BROS (Biggyani Researcher OS):** A research-oriented environment built on the BOS foundation.
- **Kolpona:** A separate VR/AR and Digital Twin environment.

These projects are outside the current BOS implementation scope. Their future development must not unnecessarily complicate the initial BOS architecture.

## 11. Current Development Scope

The immediate objective is not to build a complete independent operating system from scratch.

The current development scope is:

1. Establish the Debian-based development environment.
2. Build a bootable BOS prototype.
3. Make the prototype installable in VirtualBox.
4. Configure and customize the desktop environment.
5. Validate basic operation, networking, and offline functionality.
6. Establish documentation and repeatable build procedures.
7. Progressively introduce independent BOS components.

## 12. Long-Term Architectural Direction

BOS will evolve through incremental development.

The long-term direction is an independently identifiable Linux-based operating system with:

- Its own branding and system identity.
- Its own desktop environment.
- Custom system utilities.
- A maintainable component architecture.
- A reliable installation and packaging process.
- Broad hardware compatibility.
- Offline-first functionality.

The architecture will evolve as development and testing produce evidence for necessary changes.

---

**Document status:** Initial architecture foundation.  
**Project:** Biggyani OS (BOS).
