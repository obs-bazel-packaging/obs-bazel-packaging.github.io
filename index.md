**Unofficial** packaging for [Bazel build system](https://bazel.build/) with focus on ARM64 builds.
All repositories provide x86_64 and aarch64 builds and are hosted on the [openSUSE Open Build System](https://build.opensuse.org/) instance, in [this project](https://build.opensuse.org/project/show/home:mrostecki:bazel).

## Debian

### Stable 10 (Buster)

```
# echo "deb https://download.opensuse.org/repositories/home:/mrostecki:/bazel/Debian_10/ /" > /etc/apt/sources.list.d/bazel.list
# curl -L https://download.opensuse.org/repositories/home:/mrostecki:/bazel/Debian_10/Release.key | apt-key add -
# apt update
# apt install bazel
```

### Testing

```
# echo "deb https://download.opensuse.org/repositories/home:/mrostecki:/bazel/Debian_Testing/ /" > /etc/apt/sources.list.d/bazel.list
# curl -L https://download.opensuse.org/repositories/home:/mrostecki:/bazel/Debian_Testing/Release.key | apt-key add -
# apt update
# apt install bazel
```

### Unstable

```
# echo "deb https://download.opensuse.org/repositories/home:/mrostecki:/bazel/Debian_Unstable/ /" > /etc/apt/sources.list.d/bazel.list
# curl -L https://download.opensuse.org/repositories/home:/mrostecki:/bazel/Debian_Unstable/Release.key | apt-key add -
# apt update
# apt install bazel
```

## openSUSE

Bazel package is available for openSUSE Tumbleweed in official repos, also for aarch64.
Installation is as easy as:

```
# zypper install bazel
```

## Ubuntu

### Ubuntu 20.04

```
# echo "deb https://download.opensuse.org/repositories/home:/mrostecki:/bazel/xUbuntu_20.04/ /" > /etc/apt/sources.list.d/bazel.list
# curl -L https://download.opensuse.org/repositories/home:/mrostecki:/bazel/xUbuntu_20.04/Release.key | apt-key add -
# apt update
# apt install bazel
```

## Support or Contact

Having troubles with those repositories or packages? [Contact me](mrostecki@opensuse.org)

## TODO

- Store all files (`debian.*` and `*.spec`) needed for package builds on Github, then synchronize them to OBS, to make contributions easier.
- More architectures (ppc, s390x).
