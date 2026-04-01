# Immutable Linux Distributions

## Fully Immutable (read-only root)

| Distro | Base | Notes |
|--------|------|-------|
| **NixOS** | Independent | Declarative config, atomic rollbacks |
| **Fedora Silverblue** | Fedora/RPM | GNOME desktop, rpm-ostree |
| **Fedora Kinoite** | Fedora/RPM | KDE desktop, rpm-ostree |
| **Fedora Sericea** | Fedora/RPM | Sway desktop, rpm-ostree |
| **Fedora Onyx** | Fedora/RPM | Budgie desktop, rpm-ostree |
| **Universal Blue (uCore, Bazzite, etc.)** | Fedora/OCI | Custom images built on Silverblue |
| **SteamOS 3** | Arch | Immutable root, Valve's gaming OS |
| **openSUSE MicroOS** | openSUSE | Server/container focus |
| **openSUSE Aeon** | openSUSE | Desktop variant of MicroOS |
| **Vanilla OS** | Ubuntu/Debian | Uses ABRoot for dual-partition A/B |
| **blendOS** | Arch | Container-based apps |
| **carbonOS** | Independent | OCI-based, GNOME |

## Mostly Immutable / Atomic Update Systems

| Distro | Notes |
|--------|-------|
| **Chrome OS / ChromiumOS** | A/B partition updates, verified boot |
| **endless OS** | OSTree-based, offline-first |
| **GNOME OS** | Reference platform, OSTree |
| **Bottlerocket** | AWS's container host OS |
| **Flatcar Container Linux** | CoreOS successor, server/container |
| **Talos Linux** | Kubernetes-focused, API-managed |

## Key Technologies Behind Them

- **OSTree / rpm-ostree** — Fedora ecosystem
- **Nix store** — NixOS
- **ABRoot** — Vanilla OS
- **A/B partitions** — Chrome OS, SteamOS, Bottlerocket
- **SquashFS + overlayfs** — live-system style immutability
