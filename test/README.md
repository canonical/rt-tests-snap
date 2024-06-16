# RT-tests smoke tests 

These are smoke tests that check if the main functionalities of each program
are working. This is done by using regular expressions (RegEx) to check
if the output matches the expected behavior for a given command and its
arguments.


## Running tests

To run the tests, execute the `run` script with root priviledges:

`sudo ./run`

Specifically for the snap installation, it’s necessary to create some
manual aliases:

```bash
sudo snap alias rt-tests.cyclictest cyclictest
sudo snap alias rt-tests.cyclicdeadline cyclicdeadline 
sudo snap alias rt-tests.deadlinetest deadline_test
sudo snap alias rt-tests.get-cyclictest-snapshot get-cyclictest-snapshot
sudo snap alias rt-tests.hackbench hackbench
sudo snap alias rt-tests.hwlatdetect hwlatdetect
sudo snap alias rt-tests.oslat oslat
sudo snap alias rt-tests.pip-stress pip_stress
sudo snap alias rt-tests.pi-stress pi_stress
sudo snap alias rt-tests.pmqtest pmqtest
sudo snap alias rt-tests.ptsematest ptsematest
sudo snap alias rt-tests.queuelat queuelat
sudo snap alias rt-tests.rt-migrate-test rt-migrate-test
sudo snap alias rt-tests.signaltest signaltest
sudo snap alias rt-tests.sigwaittest sigwaittest
sudo snap alias rt-tests.ssdd ssdd
sudo snap alias rt-tests.svsematest svsematest
```
