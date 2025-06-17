## Test instructions

To test, go to the `kvraft` folder, and run:
- `go test -run 5A`.

To test for data races, go to the `kvraft` folder and run:
- `go test -race -run 5A`.

To profile, go to the `kvraft` folder and run:
- `go test -race -run 5A -cpuprofile=cpu.out -mutexprofile=mutex.out`.

There is intense logging for debugging, to disable logging run:
- `export LOGGER_OVERRIDE=True` before the test suite.
- Logging can be re-enabled by running `unset LOGGER_OVERRIDE`.

Please note that these tests and this assignment are derived from the MIT 6.824 lab 3A, adapted for UBC CPSC416:
http://nil.csail.mit.edu/6.824/2022/labs/lab-kvraft.html
