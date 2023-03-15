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
| %n | Newline | ('\n') |	
| %p | Morning AM or Afternoon PM | PM |
| %r | Full 12-hour time (HH:MM:SS | 01:23:45 PM |
| %R | 24-hour time (HH:MM) | 12:30 |
| %S | Seconds (Zero-padded) (00-61) | 01 |
| %s	Unix time; the number of seconds since the Unix epoch.	1455803239
| %t	Horizontal-tab character ('\t')	
| %T	ISO 8601 time format (HH:MM:SS), equivalent to %H:%M:%S	18:25:34
| %u	ISO 8601 weekday as number with Monday as 1 (1-7)	6
| %U	Week number with the first Sunday as the first day of week one (00-53)	30
| %V	ISO 8601 week number (00-53)	12
| %w	Weekday as a decimal number with Sunday as 0 (0-6)	5
| %W	Week number with the first Monday as the first day of week one (00-53)	50
| %x	National date representation	05/28/11
| %X	National time representation	12:22:02
| %y	Year, last two digits (00-99)	11
| %Y	Year	2016
| %z	The time zone offset from UTC; a leading plus sign stands for east of UTC, a minus sign for west of UTC, hours and minutes follow with two digits each and no delimiter between them. If timezone cannot be determined, no characters.	+0100
| %Z	Timezone name or abbreviation; if timezone cannot be determined, no characters	CEST

## Return Value
Ctime.format() returns a date formatted string

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
