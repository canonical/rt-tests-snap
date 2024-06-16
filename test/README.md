# RT-tests smoke tests 

These are smoke tests that check if the main functionalities of each program
are working. This is done by using regular expressions (RegEx) to check
if the output matches the expected behavior for a given command and its
arguments.


## Running tests

To run the tests, execute the `run` script with root privileges:

```bash
sudo ./run
```

For testing the snap, it’s necessary to remove the Debian package (if installed) and alias the snapped applications beforehand:

```bash
sudo apt remove rt-tests
./alias-snap-apps
```
