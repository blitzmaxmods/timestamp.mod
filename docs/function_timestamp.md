# Timestamp()

## Syntax
```Function Timestamp:Long()``` 

## Description

Timestamp() is a function that returns the number of seconds since the Unix Epoch (1 Jan 1970). It is commonly refererred to as UnixTime or a Unix Timestamp.
See also [Ctime.time()](Ctime_time.md)

## Return Value
Timestamp() returns a signed Long

## Dependencies
* [BlitzMaxNG](https://blitzmax.org)
* [bmx.timestamp](..README.md)

## Threadsafe
Has not been evaluated, but all the C functions used have been confirmed

## Example
```
Import bmx.timestamp

Local time:Long = Timestamp()
```

## Further Reading
* [BlitzMaxNG](https://blitzmax.org)
* Module [bmx.timestamp](../README.md)

