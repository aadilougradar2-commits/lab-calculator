# Calculator lab project

## Prerequisites
- Python 3 must be installed.

## How to run it
1. Open a terminal in the calculator folder.
2. Run the startup script:

   ./run.sh

## Sample test
Enter the following values:
- First number: 6
- Operator: *
- Second number: 7

Expected result:

Result: 42.0

## How to stop
Press Ctrl + C in the terminal.

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
