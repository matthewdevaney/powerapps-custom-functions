# Matthew Devaney's Function Library
Functions that perform operations on a date value
* [Date Functions](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#Date-Functions)
* [Financial Functions](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#Financial-Functions)
</br></br>

# Date Functions
Functions that perform operations on a date value
* [EndOfQuarter](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#EndOfQuarter)
* [EndOfMonth](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#EndOfMonth)
* [EndOfWeek](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#EndOfWeek)
* [EndOfYear](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#EndOfYear)
* [NetWorkDays](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#NetWorkDays)
* [StartOfQuarter](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#StartOfQuarter)
* [StartOfMonth](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#StartOfMonth)
* [StartOfWeek](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#StartOfWeek)
* [StartOfYear](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#StartOfYear)
* [WeekNumber](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#WeekNumber)
* [YearFraction](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#YearFraction)
</br></br>

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
Get the last day of a week.
### Syntax
EndOfWeek(StartDate [, AddWeeks, DayWeekStart])
* StartDate: Required
* AddWeeks: Optional
* DayWeekStart: Optional
</br></br>


## EndOfYear
Get the last day of a year.
### Syntax
EndOfYear(StartDate [, AddYears])
* StartDate: Required
* AddYears: Optional
</br></br>


## NetWorkDays
Find the number of work days between two dates.
### Syntax
NetWorkDays(StartDate, EndDate)
* StartDate: Required
* EndDate: Required
</br></br>


## StartOfMonth
Get the first day of a month.
### Syntax
StartOfMonth(StartDate [, AddMonths])
* StartDate: Required
* AddMonths: Optional
</br></br>


## StartOfQuarter
Get the first day of a quarter.
### Syntax
StartOfQuarter(StartDate [, AddQuarters])
* StartDate: Required
* AddQuarters: Optional
</br></br>


## StartOfWeek
Get the first day of a week.
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
Takes a date and returns a week number (1-54) that corresponds to the week of year.
### Syntax
WeekNumber(StartDate [,DayWeekStart])
* StartDate: Required
* DayWeekStart: Optional
</br></br>


## YearFraction
Calculates a decimal number representing the fraction of a year between two dates.
### Syntax
YearFraction(StartDate, EndDate [,DayWeekStart])
* StartDate: Required
* EndDate: Required
* Basis: Optional
</br></br>



# Financial Functions
functions that are used by accounting & finance
* [FV](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#FV)
* [PV](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#PV)
* [NPER](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#NPER)
* [PMT](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#PMT)
</br></br>



## FV
future value: a cash balance you want to attain after the last payment is made.
### Syntax
PV(Rate, NPER, PMT [, PV])
* Rate: Required
* NPER: Required
* PMT: Required
* PV: Optional
</br></br>


## PV
present value: the total amount that a series of future payments is worth now
### Syntax
PV(Rate, NPER, PMT [, FV])
* Rate: Required
* NPER: Required
* PMT: Required
* FV: Optional
</br></br>


## NPER
the total number of payments for a loan
### Syntax
NPER(Rate, PMT, PV [, FV])
* Rate: Required
* PMT: Required
* PV: Required
* FV: Optional
</br></br>


## PMT
the payment made each period over the life of an investment.
### Syntax
PV(Rate, NPER, PV [, FV])
* Rate: Required
* NPER: Required
* PV: Required
* FV: Optional
</br></br>
