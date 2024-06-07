
# Real Time Tests Snap 

[![real-time-tests](https://snapcraft.io/real-time-tests/badge.svg)](https://snapcraft.io/real-time-tests)

This is the snap packaging o
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
