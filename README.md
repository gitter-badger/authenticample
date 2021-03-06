# Authenticample
## Build instructions:

    $ git submodule init
    $ git submodule update
    $ mkdir build
    $ cd build
    $ cmake ..
    $ make

## Running server:

    $ src/server/server <port>

To use with SSL support, use the following format of the port number:

[ssl://][host:]port[:server certificate with private key file in PEM format[:CA certificate]]

For example:

    $ server ssl://127.0.0.1:8043:server.pem:cacert.pem

## Running client:

    $ client [-u <URL>] [-c <client's cert file> -k <client's private key file>] [-r <CA certs file>]

[![Build Status](https://travis-ci.org/kvirund/authenticample.svg?branch=master)](https://travis-ci.org/kvirund/authenticample)
