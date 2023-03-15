# Ctime.time()

## Syntax
```Ctime.format:String( dateformat:String=DT_DATETIME )``` 

## Description

Ctime.format() is a method of Struct [Ctime](Ctime.md) and returns a string representation of  the date in a given date format.

Some constants have been provided, but you can create your own using standard strfformat codes as listed below:

See also:
* [Ctime.Dayname()](Ctime_dayname.md)
* [Ctime.Monthname()](Ctime_monthname.md)

**DateFormat Constants**

|**CONSTANT**|**FORMAT**|
|---|---|
| DT_DATETIME | %Y-%m-%d %H:%M:%S |
| DT_DATE | %Y-%m-%d |
| DT_TIME | %H:%M:%S |
| DT_DATESTR | %d %b %Y |
| DT_AMERICAN | %m %d %Y |
| DT_BRITISH | %d %m %Y |
| MYSQL_DATE | DT_DATE |
| MYSQL_DATETIME | DT_DATETIME |
| MYSQL_TIMESTAMP | DT_DATETIME |
| MYSQL_YEAR | %Y |
| MSSQL_DATE | DT_DATE |
| MSSQL_DATETIME | DT_DATETIME |
| MSSQL_TIMESTAMP| % |
| MSSQL_SMALLDATETIME | DT_DATETIME

**NOTE**: A simple "%" as a dateformat will render the unix timestamp as a string (See MSSQL_TIMESTAMP).

**Dateformat Codes**
|**CODE**|**DESCRIPTION**|**EXAMPLE**|
|---|---|
| %% | The % Character | %% |
| %a | Short weekday name | Mon |
| %A | Full weekday name | Monday |
| %b | Short month name | Oct |
| %B | Full month name | October |
| %c | Locale date representation | |
| %C | Two digit Century (00 to 99) | 20 |
| %d | Day of Month (Zero-padded) (01-31) | 03 |
| %e | Day of month (Space padded) ( 1-31) | " 1" |
| %H | Hour (24h format) (00-23) | 22 |
| %I | Hour (12h format) (01-12) | 10 |
| %j | Day of the year (1-366) | 123 |
| %m | Month (Zero-padded) (01-12) | 06 |
| %M | Minute (Zero-padded) (00-59)	52
| %n | Newline | "\n" |	
| %p | Morning AM or Afternoon PM | PM |
| %r | Full 12-hour time (HH:MM:SS | 01:23:45 PM |
| %R | 24-hour time (HH:MM) | 12:30 |
| %S | Seconds (Zero-padded) (00-61) | 01 |
| %s | Unix timestamp | 1678898701 |
| %t | Tab | "\t" |	
| %T | ISO 8601 format (HH:MM:SS) | 15:45:22 |
| %u | ISO 8601 weekday (1-7) | 2 |
| %U | Week number (Sunday bias) (00-53) | 50 |
| %V | ISO 8601 week number (00-53) | 50 |
| %w | Weekday (Sunday bias) (0-6) | 4 |
| %W | Week number (Monday bias) (00-53) | 50 |
| %x | National date ||
| %X | National time ||
| %y | Year (Two digit) (00-99) | 43 |
| %Y | Year	(Four digit) | 1943 |
| %z | Time zone relative to UTC ||
| %Z | Timezone name ||

## Return Value
Ctime.format() returns a date formatted string

## Dependencies
* [BlitzMaxNG](https://blitzmax.org)

## Threadsafe
Has not been evaluated, but all the C functions used have been confirmed

## Example
```
Import bmx.timestamp

Local time:Ctime = new Ctime()
Print time.format()

```

## Further Reading
* [BlitzMaxNG](https://blitzmax.org)
* Module [bmx.timestamp](../README.md)
* Struct [Ctime](Ctime.md)
