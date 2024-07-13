This is a custom BlendOS track customized to my liking.

It adds virt-manager with all qemu platforms like arm64, x86-64 etc. It also removes everything except the utilities and console. So you only get the BARE minimum. Not even firefox is included. It also creates the needed groups for qemu to function properly. Waydroid is also stripped out. The GNOME desktop is kept ofc.

If you would like a more detailed explanation, here's a summary provided by ChatGPT:

This file is a configuration file for BlendOS V4, specifically a `system.yaml` file that describes the system setup and package requirements. Here's a detailed explanation of its contents:

### Overview

- **impl**: Specifies the URL for the implementation of the `track`, which is `blendos-base`.
- **track**: Indicates the track or the base system image being used, which is `blendos-base`.

### Packages

The `packages` section lists the packages that need to be installed from the BlendOS repository. Here’s a brief description of some of them:

- **adw-gtk3**: Adwaita theme for GTK 3 applications.
- **baobab**: Disk usage analyzer.
- **blendos-wallpapers-git**: Wallpaper package for BlendOS.
- **gdm**: GNOME Display Manager.
- **gnome-backgrounds**: Background images for GNOME.
- **gnome-calculator**: Calculator application.
- **gnome-console**: Terminal emulator.
- **gnome-control-center**: GNOME's system settings.
- **gnome-disk-utility**: Disk management utility.
- **gnome-keyring**: Secure key storage.
- **gnome-menus**: GNOME menu system.
- **gnome-session**: GNOME session management.
- **gnome-settings-daemon**: Manages GNOME settings.
- **gnome-shell**: GNOME desktop environment.
- **gnome-shell-extensions**: Extensions for GNOME Shell.
- **gnome-software**: Software management tool.
- **gnome-system-monitor**: System monitor application.
- **gnome-text-editor**: Text editor.
- **gnome-user-docs**: User documentation for GNOME.
- **gnome-user-share**: User file sharing service.
- **grilo-plugins**: Media discovery framework.
- **gvfs**: Virtual file system service.
- **gvfs-afc**: AFC (Apple File Conduit) support for GVFS.
- **gvfs-goa**: GNOME Online Accounts integration for GVFS.
- **gvfs-google**: Google Drive integration for GVFS.
- **gvfs-gphoto2**: gPhoto2 (digital camera) support for GVFS.
- **gvfs-mtp**: MTP (Media Transfer Protocol) support for GVFS.
- **gvfs-nfs**: NFS (Network File System) support for GVFS.
- **gvfs-smb**: SMB (Samba) support for GVFS.
- **loupe**: GNOME image viewer.
- **malcontent**: Parental control.
- **nautilus**: GNOME file manager.
- **orca**: Screen reader.
- **rygel**: DLNA/UPnP media server.
- **snapshot**: Camera app.
- **tecla**: Not specified.
- **tracker3-miners**: Metadata database, indexer, and search tool.
- **xdg-desktop-portal-gnome**: GNOME backend for xdg-desktop-portal.
- **xdg-user-dirs-gtk**: User directories handling for GTK.
- **gnome-shell-extension-blur-my-shell**: Extension for blurring the GNOME Shell background.
- **gnome-shell-extension-appindicator**: Extension for supporting app indicators in GNOME Shell.
- **gnome-shell-extension-dash-to-dock**: Extension for turning the GNOME dash into a dock.
- **gnome-initial-setup**: First-time setup tool for GNOME.

### AUR Packages

The `aur-packages` section lists packages to be installed from the Arch User Repository (AUR):

- **qemu-full**: Full installation of QEMU, a hardware virtualization tool.
- **virt-manager**: Manager for virtual machines.

### Commands

The `commands` section contains commands to be executed, such as:

- Removing specific metainfo files and desktop entries that are not needed.
- Managing users and groups, particularly for setting up libvirt and QEMU.

### Services

The `services` section lists the services to be enabled:

- **gdm**: GNOME Display Manager.
- **libvirtd**: Libvirt daemon for managing virtualization.
- **libvirt-storaged**: Storage management daemon for libvirt.

### Summary

This `system.yaml` file is used to configure a BlendOS V4 system with a GNOME desktop environment, necessary tools, and virtualization capabilities. It defines the required packages, custom commands to execute, and services to enable, ensuring the system is set up according to the specified requirements.
