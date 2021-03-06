# SRFI 117 - Mutable Queues

This repository hosts a reference implementation of SRFI 117 - Mutable Queues. The full documentation for this SRFI can be found on the [SRFI Document Reference](http://srfi.schemers.org/srfi-117). The repository hosts a complete implementation of the SRFI, running on [CHICKEN](http://call-cc.org) Scheme.

## File Description

While this repository is primarily to provide a reference implementation of SRFI 117, it also currently serves as the base repository to host the library as a CHICKEN extension (egg). Thus, there are three files that are independent of the SRFI itself, and are as follows:

`srfi-117.meta`
: This file denotes metadata about the CHICKEN extension, such as author, license, and dependencies (and dependencies for tests).

`srfi-117.setup`
: This file tells the CHICKEN package manager (`chicken-install`) how to build the egg.

`srfi-117.release-info`
: Describes the URL / different releases of the CHICKEN extension.

Additionally, the `tests/` directory has been added to accommodate the CHICKEN package manager (for running tests). Currently it provides a default test runner which merely includes the tests found in the `list-queues/` directory.

## License

Provided under a single clause BSD license, Copyright (C) John Cowan 2015. See LICENSE for full details.

