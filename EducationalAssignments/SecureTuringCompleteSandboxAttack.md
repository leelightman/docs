
# Secure Turing Complete Sandbox Challenge -- Attacking Sandboxes

The second part of the Secure Turing Complete Sandbox Challenge is to try to break the security of candidate sandboxes.   While not all bugs may be exploitable, it is worth documenting any problems that may arise in case another attacker can use them to find a way to escape sandbox containment.






## Acquiring Sandboxes
----

There should be a series of publicly available sandboxes including the ones attached to this wiki page.   Other links will be provided here to those sandboxes.




## Hint: Look For Corner Cases
----

Many flaws deal with incorrect handling of corner cases.   Try to find any situations where the behavior of the sandbox is not well specified.   Any bugs you find (whether exploitable or not) should be noted.




## What To Turn In
----

You must turn in the URL and SHA1 hash of the head of your GitHub project.   The project must contain the following:

 1. For each sandbox you were asked to analyze, explain at a high level what type of technique they used.   This should be 1-2 sentences.   For example: The easytocode.py sandbox is written in Python.   It filters input programs (written in a subset of Python) for disallowed strings, replaces the module / built-ins namespace, and execs the code.   Please provide this in PDF format.
 1. Any test files that crash the sandbox in unexpected ways.   The test program must have documentation explaining how the crash is generated.   Please turn in a separate file per unique class of bug found.   (In other words, if a program crashes when given negative numbers or floating point numbers, turn in a test case with -1 and one with 1.0.   Don't turn in separate cases for -1, -2, -3, ...)   If the source code format does not allow for comments, please add these in a separate file called README.testname.
 1. Any test files that allow escape of the sandbox, including performing actions that were not allowed.   As before, please turn in separate files per unique class of bug and also explain how exploits are performed.
 1. A summary file (called summary.pdf) that contains an overview of the contents of the submission.   This should say which tests go with each sandbox and also whether the tests demonstrate a crash or sandbox escape.

