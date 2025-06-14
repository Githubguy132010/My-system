# Custom BlendOS Tracks

## Overview
This is a collection of customized BlendOS tracks tailored to specific requirements, focusing on virtualization capabilities with minimal bloat. The tracks are organized into two categories: with Waydroid support and without Waydroid support.

## Track Organization

### Waydroid Tracks (`/waydroid/`)
Tracks in this folder include Waydroid support for Android app compatibility:
- **KDE.yaml** - KDE Plasma desktop with Waydroid
- **GNOME.yaml** - GNOME desktop with Waydroid
- **COSMIC.yaml** - COSMIC desktop with Waydroid

### No-Waydroid Tracks (`/no-waydroid/`)
Tracks in this folder exclude Waydroid for a lighter system:
- **KDE.yaml** - KDE Plasma desktop without Waydroid
- **GNOME.yaml** - GNOME desktop without Waydroid
- **COSMIC.yaml** - COSMIC desktop without Waydroid

> [!WARNING]
> **Do NOT install the KDE or COSMIC tracks by editing `blend-inst` in the live USB to point to these custom tracks.**
>
> This skips the user creation step entirely, resulting in a corrupted system where **no user account exists** and login becomes impossible.
>
> Instead, install the default version of BlendOS and create your user account. Then switch to the KDE or COSMIC track I created. (You can find instructions on the release page.)

> [!NOTE]
*This issue does **not** occur on GNOME variants, as they include `gnome-initial-setup` to guide user creation on first boot.*


## Features

### Added Components
- **virt-manager** with complete QEMU platform support:
  - arm64
  - x86-64
  - And other architectures
- Proper user group configurations for QEMU functionality
- Optional Waydroid support for Android applications

### Minimalist Approach
- Includes only essential utilities and console applications
- Retains the GNOME/KDE/COSMIC desktop environments
- Excludes non-essential applications (including Firefox)

## Purpose
These tracks are designed for users who want a lightweight BlendOS installation with robust virtualization capabilities without unnecessary software. Choose between tracks with or without Waydroid support based on your needs.
