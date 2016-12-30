## Miscellaneous plugins for wkfs

[wkfs](https://godoc.org/go4.org/wkfs) is a pluggable "well-known filesystem" abstraction layer.

Instead of accessing files directly through the operating system using `os.Open` or `os.Stat`, code should use `wkfs.Open` or `wkfs.Stat`, which first try to intercept paths at well-known top-level directories representing previously-registered mount types, otherwise fall through to the operating system paths.

This repo contains some miscellaneous plugins for wkfs.
