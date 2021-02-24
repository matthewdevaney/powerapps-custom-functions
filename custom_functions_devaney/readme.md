# Date Functions
Functions that perform operations on a date value</br></br>


## EndOfQuarter
Get the last day of a quarter.
### Syntax
StartOfQuarter(StartDate [, AddQuarters])
* StartDate: Required
* AddQuarters: Optional
</br></br>


## EndOfMonth
Get the last day of a month.
### Syntax
EndOfMonth(StartDate [, AddMonths])
* StartDate: Required
* AddMonths: Optional
</br></br>


## EndOfWeek
Get the last day of a week.</br></br>
### Syntax
EndOfWeek(StartDate [, AddWeeks, DayWeekStart])
* StartDate: Required
* AddWeeks: Optional
* DayWeekStart: Optional
</br></br>


## EndOfYear
Get the last day of a year.</br></br>
### Syntax
EndOfYear(StartDate [, AddYears])
* StartDate: Required
* AddYears: Optional
</br></br>


## NetWorkDays
Find the number of work days between two dates.</br></br>
### Syntax
NetWorkDays(StartDate, EndDate)
* StartDate: Required
* EndDate: Required
</br></br>


## StartOfMonth
Get the first day of a month.</br></br>
### Syntax
StartOfMonth(StartDate [, AddMonths])
* StartDate: Required
* AddMonths: Optional
</br></br>


## StartOfQuarter
Get the first day of a quarter.</br></br>
### Syntax
StartOfQuarter(StartDate [, AddQuarters])
* StartDate: Required
* AddQuarters: Optional
</br></br>


## StartOfWeek
Get the first day of a week.</br></br>
### Syntax
StartOfWeek(StartDate [, AddWeeks, DayWeekStart])
* StartDate: Required
* AddWeeks: Optional
* DayWeekStart: Optional
</br></br>


## StartOfYear
Get the first day of a year.
### Syntax
StartOfYear(StartDate [, AddYears])
* StartDate: Required
* AddYears: Optional
</br></br>


## WeekNumber
Takes a date and returns a week number (1-54) that corresponds to the week of year.</br></br>
### Syntax
WeekNumber(StartDate [,DayWeekStart])
* StartDate: Required
* DayWeekStart: Optional
</br></br>


## YearFraction
Calculates a decimal number representing the fraction of a year between two dates.</br></br>
### Syntax
YearFraction(StartDate, EndDate [,DayWeekStart])
* StartDate: Required
* EndDate: Required
* Basis: Optional
</br></br>



# Financial Functions
</br></br>

## PV
present value: the total amount that a series of future payments is worth now</br></br>
### Syntax
PV(Rate, NPER, PMT [, FV])
* Rate: Required
* NPER: Required
* PMT: Required
* FV: Optional
</br></br>

## FV
future value: a cash balance you want to attain after the last payment is made* 
### Syntax
PV(Rate, NPER, PMT [, PV])
* Rate: Required
* NPER: Required
* PMT: Required
* PV: Optional
</br></br>


## PMT
the payment made each period over the life of an investment</br></br>
### Syntax
PV(Rate, NPER, PV [, FV])
* Rate: Required
* NPER: Required
* PV: Required
* FV: Optional
</br></br>

## NPER
the total number of payments for a loan
the payment made each period over the life of an investment</br></br>
### Syntax
NPER(Rate, PMT, PV [, FV])
* Rate: Required
* PMT: Required
* PV: Required
* FV: Optional
</br></br>
