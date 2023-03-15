# Ctime.time()

## Syntax
```Ctime.time:Long()``` 

## Description

Ctime.time() is a static function of the Struct [Ctime](Ctime.md) and returns the number of seconds since the Unix Epoch (1 Jan 1970). It is commonly refererred to as UnixTime or a Unix Timestamp.

See also [Timestamp()](function_timestamp.md)

## Return Value
Ctime.time() returns a signed Long

## Dependencies
* [BlitzMaxNG](https://blitzmax.org)

## Threadsafe
Has not been evaluated, but all the C functions used have been confirmed

## Example
```
Import bmx.timestamp

Local time:Long = Ctime.time()
```

## Further Reading
* [BlitzMaxNG](https://blitzmax.org)
* Module [bmx.timestamp](../README.md)
* Struct [Ctime](Ctime.md)
