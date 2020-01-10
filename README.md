release-draft-test
===========
[![Build Status](https://travis-ci.org/DANS-KNAW/release-draft-test.png?branch=master)](https://travis-ci.org/DANS-KNAW/release-draft-test)


SYNOPSIS
--------

    release-draft-test (synopsis of command line parameters)
    release-draft-test (... possibly multiple lines for subcommands)


DESCRIPTION
-----------

test how release-draft can work together with our workflow in EASY

here's a change
here's a second change
here's a third change
here's a fourth change
here's a fifth change


ARGUMENTS
---------

    Options:

       -h, --help      Show help message
       -v, --version   Show version of this program

    Subcommand: run-service - Starts RELEASE Draft Test as a daemon that services HTTP requests
       -h, --help   Show help message
    ---

EXAMPLES
--------

    release-draft-test -o value

BUILDING FROM SOURCE
--------------------
Prerequisites:

* Java 8 or higher
* Maven 3.3.3 or higher
* RPM

Steps:
    
    git clone https://github.com/rvanheest/release-draft-test.git
    cd release-draft-test 
    mvn clean install

If the `rpm` executable is found at `/usr/local/bin/rpm`, the build profile that includes the RPM 
packaging will be activated. If `rpm` is available, but at a different path, then activate it by using
Maven's `-P` switch: `mvn -Pprm install`.

Alternatively, to build the tarball execute:

    mvn clean install assembly:single
