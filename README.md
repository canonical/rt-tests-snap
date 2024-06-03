
# Real Time Tests Snap 

[![real-time-tests](https://snapcraft.io/real-time-tests/badge.svg)](https://snapcraft.io/real-time-tests)

[![Get it from the Snap Store](https://snapcraft.io/static/images/badges/en/snap-store-black.svg)](https://snapcraft.io/real-time-tests)

This is the snap packaging of
[rt-tests](https://wiki.linuxfoundation.org/realtime/documentation/howto/tools/rt-tests).



## Install

To install it:

```bash
sudo snap install real-time-tests
```

## Configure

It's necessary to connect the interface [process-control](https://snapcraft.io/docs/process-control-interface) to work properlly:

```bash
sudo snap connect real-time-tests:process-control :process-control
```

### Local Build

```bash
snapcraft -v

sudo snap install --dangerous *.snap
```