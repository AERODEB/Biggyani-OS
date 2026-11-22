# Biggyani OS (BOS) — Live ISO Boot Test Report

**Project:** Biggyani OS (BOS)  
**Test stage:** Initial Live ISO boot validation  
**Test date:** 2026-11-22  
**Test environment:** VirtualBox virtual machine `BOS-LIVE-TEST`  
**Base distribution:** Debian GNU/Linux 13 (Trixie), amd64  
**Desktop environment:** KDE Plasma  
**Test result:** PASS — 8 of 8 checks passed

---

## 1. Test Objective

Verify that the first Debian-based Biggyani OS Live ISO boots in VirtualBox and provides a usable graphical Live session without installing the system to the virtual disk.

## 2. Tested Image

| Property | Recorded value |
|---|---|
| ISO filename | `biggyani-os-amd64.hybrid.iso` |
| Build system | Debian Live Build |
| Live-build version shown at boot | `20250505+deb13u1` |
| Linux kernel shown at boot | `6.12.117-1` |
| Live-boot version shown at boot | `1:20250815~deb13u1` |
| Live-config version shown at boot | `11.0.5` |
| Live-tools version shown at boot | `1:20240525` |
| SHA-256 | `b6d10f746a3d28e1e7b0a4888430502040fec65bbc05f0abdcb443371281323c` |

The SHA-256 was checked after copying the ISO to the Windows shared folder and matched the original build's recorded checksum.

## 3. Test Results

| # | Test | Result |
|---:|---|---|
| 1 | KDE Plasma desktop loads successfully | PASS |
| 2 | Mouse and keyboard work | PASS |
| 3 | Display resolution is correct | PASS |
| 4 | Applications menu opens | PASS |
| 5 | File manager opens | PASS |
| 6 | Terminal opens | PASS |
| 7 | Network connection works | PASS |
| 8 | System can shut down and restart | PASS |

**Overall result: 8/8 checks passed.**

## 4. Observations

- The ISO displays the Debian GNU/Linux 13 (Trixie) boot menu.
- The normal amd64 Live system option boots successfully.
- KDE Plasma starts and displays its first-run welcome/configuration wizard.
- The Live session uses the default `debian` Live user.
- The current image retains Debian branding and default Live-session identity. BOS-specific branding and user configuration have not yet been implemented.
- The system was tested as a Live environment. No installation was performed.

## 5. Scope and Limitations

This test validates the initial Live boot and the eight functions listed above in VirtualBox only.

The following have **not** been established by this test:
- Installation to a virtual or physical disk.
- Independent boot of an installed BOS system.
- Physical-hardware compatibility.
- Offline operation.
- Audio functionality.
- Package installation and update behavior.
- A customized BOS desktop identity or first-boot experience.

The ISO is therefore a **bootable Live prototype**, not yet an installable BOS release.

## 6. Next Milestone

Proceed to the installer-integration stage:

1. Preserve this Live-only ISO as the validated baseline.
2. Configure Debian Installer integration for the next image.
3. Build a new ISO with Live and installation functionality.
4. Test installation using the separate `BOS-LIVE-TEST` virtual disk.
5. Verify that the installed system boots independently after installation media is detached.

Do not treat the current Live-only image as an installer.

---

**Record status:** Completed test report  
**Project:** Biggyani OS (BOS)
