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


Included plugins
This build includes 13 plugins from the original suite:

ChannelBox
Convolution
FilmGrade
FreqEQ
FreqSep
HueConverge
Matrix
Qualifier
Replace
ResolveMath
ResolveMathxtra
Scan
SoftClip

Not included
ACES and VideoGrade are not included in this build. Both load and
build correctly but fail to initialize in current DaVinci Resolve versions
(an internal incompatibility in their plugin description that is independent
of the Apple Silicon port). ACES is also largely superseded by Resolve's
built-in ACES 2.0 color management. They may be revisited in a future build.


Credits:
Original plugins and source: Paul Dore (baldavenger) —
https://github.com/baldavenger
