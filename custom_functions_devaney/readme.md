# Date Functions
Functions that perform operations on a date value</br></br>

## DateMonthEnd
Get the last day of a month.
### Syntax
DateMonthEnd(StartDate [, AddMonths])
* StartDate: Required
* AddMonths: Optional
</br></br>

## DateMonthStart
Get the first day of a month.
### Syntax
DateMonthStart(StartDate [, AddMonths])
* StartDate: Required
* AddMonths: Optional
</br></br>

## DateNetWorkDays
Find the number of work days between two dates.
### Syntax
DateNetWorkDays(StartDate, EndDate)
* StartDate: Required
* EndDate: Required
</br></br>

## DateWeekEnd
Get the last day of a week.</br></br>
### Syntax
DateWeekEnd(StartDate [, AddWeeks, DayWeekStart])
* StartDate: Required
* AddWeeks: Optional
* DayWeekStart: Optional
</br></br>

## DateWeekNum
Takes a date and returns a week number (1-54) that corresponds to the week of year
### Syntax
DateWeekEnd(StartDate [,DayWeekStart])
* StartDate: Required
* DayWeekStart: Optional
</br></br>


## DateWeekStart
Get the first day of a week.</br></br>
### Syntax
DateWeekStart(StartDate [, AddWeeks, DayWeekStart])
* StartDate: Required
* AddWeeks: Optional
* DayWeekStart: Optional
</br></br>

## DateYearEnd
Get the last day of a year.
### Syntax
DateWeekEnd(StartDate [, AddYears])
* StartDate: Required
* AddYears: Optional
</br></br>


## DateYearStart
Get the first day of a year.
### Syntax
DateWeekEnd(StartDate [, AddYears])
* StartDate: Required
* AddYears: Optional
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
