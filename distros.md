# Immutable Linux Distributions

## Fully Immutable (read-only root)

| Distro | Base | Website | Notes |
|--------|------|---------|-------|
| **NixOS** | Independent | [nixos.org](https://nixos.org) | Declarative config, atomic rollbacks |
| **Fedora Silverblue** | Fedora/RPM | [fedoraproject.org/silverblue](https://fedoraproject.org/silverblue) | GNOME desktop, rpm-ostree |
| **Fedora Kinoite** | Fedora/RPM | [fedoraproject.org/kinoite](https://fedoraproject.org/kinoite) | KDE desktop, rpm-ostree |
| **Fedora Sericea** | Fedora/RPM | [fedoraproject.org/sericea](https://fedoraproject.org/sericea) | Sway desktop, rpm-ostree |
| **Fedora Onyx** | Fedora/RPM | [fedoraproject.org/onyx](https://fedoraproject.org/onyx) | Budgie desktop, rpm-ostree |
| **Universal Blue (uCore, Bazzite, etc.)** | Fedora/OCI | [universal-blue.org](https://universal-blue.org) | Custom images built on Silverblue |
| **SteamOS 3** | Arch | [store.steampowered.com/steamos](https://store.steampowered.com/steamos) | Immutable root, Valve's gaming OS |
| **openSUSE MicroOS** | openSUSE | [microos.opensuse.org](https://microos.opensuse.org) | Server/container focus |
| **openSUSE Aeon** | openSUSE | [aeondesktop.org](https://aeondesktop.org) | Desktop variant of MicroOS |
| **Vanilla OS** | Ubuntu/Debian | [vanillaos.org](https://vanillaos.org) | Uses ABRoot for dual-partition A/B |
| **blendOS** | Arch | [blendos.co](https://blendos.co) | Container-based apps |
| **carbonOS** | Independent | [carbon.sh](https://carbon.sh) | OCI-based, GNOME |

## Mostly Immutable / Atomic Update Systems

| Distro | Website | Notes |
|--------|---------|-------|
| **Chrome OS / ChromiumOS** | [chromium.org/chromium-os](https://www.chromium.org/chromium-os) | A/B partition updates, verified boot |
| **endless OS** | [endlessos.org](https://endlessos.org) | OSTree-based, offline-first |
| **GNOME OS** | [os.gnome.org](https://os.gnome.org) | Reference platform, OSTree |
| **Bottlerocket** | [github.com/bottlerocket-os](https://github.com/bottlerocket-os/bottlerocket) | AWS's container host OS |
| **Flatcar Container Linux** | [flatcar.org](https://www.flatcar.org) | CoreOS successor, server/container |
| **Talos Linux** | [talos.dev](https://www.talos.dev) | Kubernetes-focused, API-managed |

## Key Technologies Behind Them

- **OSTree / rpm-ostree** — Fedora ecosystem
- **Nix store** — NixOS
- **ABRoot** — Vanilla OS
- **A/B partitions** — Chrome OS, SteamOS, Bottlerocket
- **SquashFS + overlayfs** — live-system style immutability
