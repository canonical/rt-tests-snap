
# Real Time Tests Snap 

[![rt-tests](https://snapcraft.io/rt-tests/badge.svg)](https://snapcraft.io/rt-tests)

[![Get it from the Snap Store](https://snapcraft.io/static/images/badges/en/snap-store-black.svg)](https://snapcraft.io/rt-tests)

This is the snap packaging of
[rt-tests](https://wiki.linuxfoundation.org/realtime/documentation/howto/tools/rt-tests).



## Install

To install it:

```bash
sudo snap install rt-tests
```

## Configure

It's necessary to connect the [process-control](https://snapcraft.io/docs/process-control-interface) interface to work properly:

```bash
sudo snap connect rt-tests:process-control :process-control
```

### Local Build

```bash
snapcraft -v

sudo snap install --dangerous *.snap
```
