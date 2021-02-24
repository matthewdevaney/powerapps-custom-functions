# Geetha Sivasailam's UDF Library
Functions that performs regex match on currency, percent & time formats
* [RegexUtils](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_geetha#Regex-Utils)
</br></br>

# Regex Utils
Functions that perform operations on a date value
* [IsCurrency](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_geetha#IsCurrency)
* [IsPercent](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_geetha#IsPercent)
* [IsTime](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_geetha#IsTime)
</br></br>

## IsCurrency
Regex to validate currency format (US)
### Syntax
IsCurrency(CurrencyTxt)
* CurrencyTxt: Required
### Output
* Boolean
</br></br>


## IsPercent
Regex to validate percent format
### Syntax
IsPercent(PercentTxt)
* PercentTxt: Required
### Output
* Boolean
</br></br>


## IsTime
Regex to validate time format [hh:mm:ss]/[h:m:s]/[mm:ss]/[m:s]/[ss]/[s]
### Syntax
IsTime(TimeTxt)
* TimeTxt: Required
### Output
* Boolean
</br></br>
