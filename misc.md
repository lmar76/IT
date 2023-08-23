# Miscellaneous topics

## Changelog file

https://keepachangelog.com/

## Diagrams

- Mermaid: https://mermaid.js.org/
- PlantUML: https://plantuml.com/
- HackerDraw: https://www.hackerdraw.com

## File Managers

### Terminal-based

- Vifm:
  * Main page: https://vifm.info/
  * Tutorial: https://wiki.vifm.info/index.php/Quickstart_Tutorial

## freedesktop.org specs

## basedir-spec

https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html

## RAM Disk

### ramdisk, ramfs, tmpfs

- https://www.kernel.org/doc/html/latest/filesystems/ramfs-rootfs-initramfs.html
- https://www.kernel.org/doc/html/latest/filesystems/tmpfs.html

### Mount a `tmpfs` volume on Linux

```
sudo mkdir -p /<path>
sudo mount -t tmpfs -o size=<size><unit-prefix> tmpfs /<path>
```

Example:
```
sudo mkdir -p /media/ramdisk
sudo mount -t tmpfs -o size=2048M tmpfs /media/ramdisk
```
