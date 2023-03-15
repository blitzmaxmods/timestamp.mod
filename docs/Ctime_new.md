# Ctime.new()

## Syntax
```
Ctime.new()
Ctime.new( dt:String, dateformat:String=DT_DATETIME )
Ctime.new( year:Int, month:Int, day:Int, hour:Int=0, minute:Int=0, second:Int=0 )
``` 

## Description

Ctime.new() is a constructor of Struct [Ctime](Ctime.md)

Pelase refer to [Ctime.Format()](Ctime_format.md) for information regarding 'dateformat' argument.

## Return Value
Ctime.new() returns a new Ctime struct

## Dependencies
* [BlitzMaxNG](https://blitzmax.org)

## Threadsafe
Has not been evaluated, but all the C functions used have been confirmed

## Example
```
Import bmx.timestamp

Local now = New Ctime()
Local xmas = New (now.year(), 12, 25 ) 
Local xmas66 = New Ctime( "1966-12-25", DT_DATE )
```

## Further Reading
* [BlitzMaxNG](https://blitzmax.org)
* Module [bmx.timestamp](../README.md)
* Struct [Ctime](Ctime.md)
