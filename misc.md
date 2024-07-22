# Miscellaneous topics

## Changelog file

<https://keepachangelog.com/>

## Diagrams

- Mermaid: <https://mermaid.js.org/>
- PlantUML: <https://plantuml.com/>
- HackerDraw: <https://www.hackerdraw.com/>

## Editors

- ecode: <https://github.com/SpartanJ/ecode>
- Lapce: <https://lapce.dev/>
- Lite: <https://github.com/rxi/lite>
- Lite XL: <https://lite-xl.com/>
- Zed: <https://zed.dev/>

## File Managers

### Terminal-based

- Vifm:
  - Main page: <https://vifm.info/>
  - Tutorial: <https://wiki.vifm.info/index.php/Quickstart_Tutorial>

## `freedesktop.org` specs

### basedir-spec

<https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html>

## Keyboard layout management

### On Linux

Command showing the available keymaps:

```text
localectl list-keymaps
```

Select a keymap from the list and run:

```text
loadkeys <map>
```

## Protocols and APIs

### STAC - SpatioTemporal Asset Catalogs

The STAC specification is a common language to describe geospatial information.

- Homepage: <https://stacspec.org/>
- STAC Index: <https://stacindex.org/>

## RAM Disk

### ramdisk, ramfs, tmpfs

- <https://www.kernel.org/doc/html/latest/filesystems/ramfs-rootfs-initramfs.html>
- <https://www.kernel.org/doc/html/latest/filesystems/tmpfs.html>

### Mount a `tmpfs` volume on Linux

```text
sudo mkdir -p /<path>
sudo mount -t tmpfs -o size=<size><unit-prefix> tmpfs /<path>
```

Example:

```text
sudo mkdir -p /media/ramdisk
sudo mount -t tmpfs -o size=2048M tmpfs /media/ramdisk
```

## Remote Desktop clients

### X11

- X2Go: <https://wiki.x2go.org/doku.php/start>

## Windows software on Linux

- Bottles: <https://usebottles.com/>
