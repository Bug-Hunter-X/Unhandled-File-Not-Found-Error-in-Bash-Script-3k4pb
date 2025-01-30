# Bash Script Error Handling Example

This repository demonstrates a common error in bash scripting: the lack of proper error handling when dealing with file operations.  The `bug.sh` script attempts to process a file that may not exist.  The `bugSolution.sh` script shows how to correctly handle the potential error.

## Bug

The `bug.sh` script directly uses `cat` without checking if the file exists. If the file doesn't exist, the command fails and the script may behave unpredictably.

## Solution

The `bugSolution.sh` script demonstrates improved error handling. It uses `-f` to check for file existence and provides informative error messages to the user.