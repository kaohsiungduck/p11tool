<!--
Copyright 2018 Thales UK Limited

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the
Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-->

# p11tool [![Build Status](https://travis-ci.com/thales-e-security/p11tool.svg?branch=master)](https://travis-ci.com/thales-e-security/p11tool)

A command line tool for interacting with [PKCS&nbsp;#11 tokens](https://en.wikipedia.org/wiki/PKCS_11). The intended 
audience is developers writing PKCS&nbsp;#11 applications who need to inspect objects, import test keys, delete 
generated keys, etc. (We wrote this tool to help with our own development projects).

## Installation

### Binaries

Binaries are available from the [releases](releases) page.

### Source installation

`dep` is required to build p11tool. See https://github.com/golang/dep#installation.

```
go get -d github.com/thales-e-security/p11tool
dep ensure --vendor-only
go install .
```

## Usage

Run `p11tool --help` to see available commands. Run `p11tool <command> --help` for help on individual commands.