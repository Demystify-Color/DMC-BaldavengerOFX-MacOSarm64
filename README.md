# DMC-BaldavengerOFX-MacOSarm64
Port of the BaldavengerOFX for MacOSarm64 (M-series, )

A macOS port of the BaldavengerOFX plugin suite (https://github.com/baldavenger/BaldavengerPlugins) for DaVinci Resolve, rebuilt as Universal Binaries so the
plugins run natively on both Apple Silicon (M1/M2/M3/M4) and Intel Macs.
The original macOS builds were compiled for Intel (x86_64) only. Because
DaVinci Resolve runs natively as an arm64 process on Apple Silicon, it could
not load those Intel-only plugins. This port fixes that by producing a single
universal binary per plugin that loads on either architecture.

Ported by Nico Fink / DeMystify Color — https://www.demystify-color.com

If you find this useful, you can support the work here:
https://buymeacoffee.com/nicofink ☕
