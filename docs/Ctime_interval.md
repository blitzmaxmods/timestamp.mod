# Ctime.interval()

## Syntax
```Function interval:Long( quantity:Int, interval:Int )``` 

## Description

Ctime.interval() is a static function of the Struct [Ctime](Ctime.md) and returns the number of seconds for the given duration.

quantity:Int  - The amount you are calculating
interval:Int  - Optional interval you are calculating (Default is seconds)

**Constants used by interval:**

|**CONSTANT**|**DETAIL**|
|---|---|
|DT_SECONDS|Interval in seconds (Default)|
|DT_MINUTES|Interval in minutes|
|DT_HOURS|Interval in hours|
|DT_DAYS|Interval in days|

## Return Value
Ctime.interval() returns a signed Long

## Dependencies
* [BlitzMaxNG](https://blitzmax.org)

## Threadsafe
Has not been evaluated, but all the C functions used have been confirmed

## Example
```
Import bmx.timestamp

Local now:Ctime = CTime.new()
Local interval:Long = Ctime.interval( 13, DT_DAYS )

now :+ interval

Print "EVENT: "+ now.format()
```

## Further Reading
* [BlitzMaxNG](https://blitzmax.org)
* Module [bmx.timestamp](../README.md)
* Struct [Ctime](Ctime.md)
