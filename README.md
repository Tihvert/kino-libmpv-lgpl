# kino-libmpv-lgpl

The LGPL libmpv Kino ships on Windows: mpv built with `-Dgpl=false`, FFmpeg without `--enable-gpl`, from the sources pinned in `versions.env`.

Build scripts adapted from [w3bward/libmpv-lgpl](https://github.com/w3bward/libmpv-lgpl) and mpv's `ci/build-mingw64.sh` (LGPL-2.1 or later, see `LICENSE`).

Build on Ubuntu 24.04 with MinGW-w64, nasm, ninja, cmake, pkg-config and meson 1.7:

```bash
./build.sh
python3 verify.py dist
```
