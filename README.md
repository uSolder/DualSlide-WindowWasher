# Window Washer

Ride the cradle up the building and wash every window.

A DualSlide game, built as a `.dsg` game file.

## Building

Needs the Arm GNU toolchain (`arm-none-eabi-gcc`), CMake 3.25 or later, Ninja,
Git and Python 3.

    cmake --preset default
    cmake --build --preset default

This fetches the [DualSlide](https://github.com/uSolder/DualSlide) game SDK at
the release named in `CMakeLists.txt` (`DUALSLIDE_VERSION`) and writes
`build/window_washer.dsg`.

To build against a DualSlide checkout beside this repository instead, while
changing the SDK and the game together, use the `local` preset:

    cmake --preset local
    cmake --build --preset local

## Installing

Connect the DualSlide to a computer, copy `window_washer.dsg` onto the DUALSLIDE
drive, and eject the drive.

## Details

| | |
| --- | --- |
| Identifier | `dualslide.window-washer` |
| Version | 1.0.0 |
