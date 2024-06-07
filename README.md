
# rt-tests snap
[![rt-tests](https://snapcraft.io/rt-tests/badge.svg)](https://snapcraft.io/rt-tests)

This is a snap packaging of
[rt-tests](https://wiki.linuxfoundation.org/realtime/documentation/howto/tools/rt-tests),
a set of programs to test various real-time Linux features. 

The programs include: 
cyclicdeadline, cyclictest, deadline_test, hackbench, oslat, pi_stress, pip_stress, pmqtest, ptsematest, queuelat, rt-migrate-test, signaltest, sigwaittest, ssdd, svsematest.


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

## Use
The program executables are available with an alias.
For example, the command for `cyclictest` is `rt-tests.cyclictest`:

On a Raspberry Pi 5 running Real-time Ubuntu 24.04:
```console
$ sudo rt-tests.cyclictest --mlockall --smp --priority=80 --interval=200 --distance=0 --loops=100000
WARN: open /dev/cpu_dma_latency: Operation not permitted
ERROR: shm_open Permission denied
policy: fifo: loadavg: 0.66 0.49 0.33 1/198 3722          

T: 0 ( 3719) P:80 I:200 C: 100000 Min:      3 Act:    5 Avg:    5 Max:      26
T: 1 ( 3720) P:80 I:200 C:  99957 Min:      2 Act:    5 Avg:    5 Max:      19
T: 2 ( 3721) P:80 I:200 C:  99919 Min:      3 Act:    6 Avg:    5 Max:      22
T: 3 ( 3722) P:80 I:200 C:  99875 Min:      3 Act:    6 Avg:    5 Max:      18
```

### Add an alias
You can add [aliases](https://snapcraft.io/docs/commands-and-aliases) to run the commands without the namespace. For example:
```console
$ sudo snap alias rt-tests.cyclictest cyclictest
Added:
  - rt-tests.cyclictest as cyclictest

$ which cyclictest
/snap/bin/cyclictest
```

### Local Build

```bash
snapcraft -v

sudo snap install --dangerous *.snap
```
