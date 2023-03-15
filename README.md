# Blitzmax Timestamp Module
VERSION 0.2 - BETA

*timestamp.mod* is a module for [BlitzMaxMG](https://Blitzmax.org) that provides a set of functions for dealing with Unix Timestamps and dates

**NOTE**

This version is a beta release and although it may be functionally complete it may not have been thorougly tested and could contain bugs.
Use at your own risk.

## Installation

Unzip and Copy timestamp.mod folder into BlitzMax/mod/bmx.mod/

On Linux:
    Open a terminal in Blitzmax/mod/bmx.mod/timestamp.mod
    ./compile.sh

On Windows
    Open a command prompt and change directory to Blitzmax\mod\bmx.mod\timestamp.mod

    cd /d C:\Blitzmax\mod\bmx.mod\timestamp.mod
    compile.bat

## Examples

Please refer to Blitzmax/mod/bmx.mod/timestamp.mod/Examples/

## Unix Timestamp

A unix timestamp is a simple number held in a Long and represents the number of seconds since the Unix Epoch (1 Jan 1970). Mostly you will find this value in system times and file dates. It is stored in BlitzMax as a Long.

To obtain the current timestamp from your system, we use CTime.time():

```Local time:Long = CTime.time()```

A helper Function called Timestamp() is also available.

# API Reference

* Function Timestamp()
* Struct [DateTime](docs/DateTime.md)

# CHANGE LOG

* 14 FEB 2023  V0.00  Draft
* 09 MAR 2023  V0.01  Draft
* 10 MAR 2023  V0.10  Beta   Fixed issue in tm structure giving stack and segmentation faults.
* 14 MAR 2023  V0.20  Beta   Changed to the internal structure to encapsulate the C struct tm

