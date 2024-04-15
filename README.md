
# Real Time Tests Snap 

[![real-time-tests](https://snapcraft.io/real-time-tests/badge.svg)](https://snapcraft.io/real-time-tests)

[![Get it from the Snap Store](https://snapcraft.io/static/images/badges/en/snap-store-black.svg)](https://snapcraft.io/real-time-tests)

This snap is based on the debian package
[rt-tests](https://wiki.linuxfoundation.org/realtime/documentation/howto/tools/rt-tests)
and it's meant to be an unofficial version of this package in snap ecosystem,
intended for use in systems that do not have any other package manager besides
snapd, specifically Ubuntu Core systems.

To install this snap, it should be installed in devmode, which requires adding
the `--devmode` flag during installation. Additionally, please note that this
snap is only available on the unstable `--edge` channel.

This snap is based on the debian package `rt-tests` and it's meant to be an
unofficial version of this package, meant to be used in systems that don't have
any other package manager besides snapd, such as Ubuntu Core systems.

## Install

As this is not avaible in store yet, it's necessary to build it locally.

### Local Build

```bash
snapcraft -v

sudo snap install --dangerous ./real-time-tests_0.1_amd64.snap
```