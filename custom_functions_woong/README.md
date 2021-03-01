// This readme is not complete. Just copied from other readme for structure

# List of components in my library

- [cmpNumbers](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_woong#cmpNumbers)
- [cmpDelayedAction](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_woong#cmpNumbers)


# cmpNumbers

Number conversions

## BinaryToDecimal
This returns Decimal value of a Binary value.

### Syntax

**BinaryToDecimal**( *Binary* )

- Binary - Required. Type: Number. Binary value. (i.e. 1000001)

### Output

Decimal value (i.e. 65)


# cmpDelayedAction

Action with a delay

## DelayedAction
This is the actions that will be triggered after delay

### Input

Set Delay input property to set the delay in milliseconds. (i.e. 1000)
Use **Reset(cmpDelayedAction)** to trigger. 

### Output

Action in DelayedAction property will be executed after delay. (i.e. Set(gblGUID(Text(GUID()))))