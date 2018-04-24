# Purpose

This repository implements an alternative buildsystem for Google's WebRTC code,
with [meson build system](http://mesonbuild.com)

The original "GN" based build system ships all required dependency itself,
including a complete toolchain, totalling at about 10GB of data that needs to be 
fetched from the internet. This makes sense to achieve reproducible builds,
and might lower problems with broken installations, or certain embedded platforms,
but is not ideal to build a custom Linux-based embedded system.

This build system tries uses as many dependencies from the system.

# Prerequisites

WebRTC requires these libraries with development files installed on your systems:

* openssl/libressl
* libopus
* alsa / libasound
* jsoncpp
* ffmpeg / libavcodec, libavutil, libavfilter
* libevent

These libraries are likely not available on your distribution, so you probably need
to clone and build/install them manually:

* libvpx (>= 1.7.0)
* OpenH264

To start generating buildfiles, type `meson . build` .
Meson will clone the other, wrapped, required libraries and check for dependencies.

To start the build, type:

    ninja -C build

# Limitations / TODO

The meson build file is currently restricted to Linux-only, tested on Debian and Alpine Linux.

* The dependency on pulseaudio is omitted, only ALSA is supported (but should still work on most PulseAudio systems)
* The Opus codec isn't advertized for an unknown reason
* Various build options and compile flags of WebRTC aren't exposed as meson options
* DTLS certificate verification is broken, checkout 'insecure' branch to ignore verification
* Support for OpenSSL 1.0 and LibreSSL is not thoroughly checked and probably leaks memory
* Build is currently non-optimized with debug symbols
* Tests and examples are not being built
