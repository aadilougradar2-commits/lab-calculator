# Calculator lab project

## How to run it

Requires Python 3.

    python3 calculator.py

Enter a first number, an operator (+ - * /) and a second number. Press Ctrl+C to stop.

## Running the tests

The tests use pytest, which is declared in requirements-dev.txt.

On the lab computers, activate the SCCM4910 virtual environment first:

    source /opt/python-venv/sccm-4910/bin/activate

Then run the local quality gate:

    ./check.sh

Expected result: 5 tests passed, then the message QUALITY GATE PASSED.

## Exit status

check.sh stops with a non-zero exit status if any test fails, and exits with status 0 only if all tests pass. Check it with `echo $?` straight after running the script. A CI job can use this status to pass or fail a build.
Operations: + - * /
