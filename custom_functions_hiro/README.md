# List of components in my library

- [ColorUtils](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_hiro#colorutils)
- [GeoUtils](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_hiro#geoutils)
- [UnitCnvt](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_hiro#unitcnvt)
- [StatUtils](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_hiro#statutils)
- [MathUtils](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_hiro#mathutils)

# ColorUtils

Convert color code to another color space (HEX to RGB, HSL to RGB, RGB to HSV etc.)

## HEX2RGB
This returns RGB values from HEX color code.

### Syntax

**HEX2RGB**( *HEX* )

- HEX - Required. Hex color code without alpha. (ex: #12abcd)

### Output

|Path|Type|Description|
|--|--|--|
|HEX2RGB( ).Color|Color|Color|
|HEX2RGB( ).R|Number|Red value|
|HEX2RGB( ).G|Number|Green value|
|HEX2RGB( ).B|Number|Blue value|

<br/>

## RGB2HSV
This converts RGB color to HSV.

### Syntax

**RGB2HSV**( *Red*, *Green*, *Blue* )

- Red - Required. Red value (0-255).
- Green - Required. Green value (0-255).
- Blue - Required. Blue value (0-255).

### Output

|Path|Type|Description|
|--|--|--|
|RGB2HSV( ).H|Number|Hue value (degree) (0-360)|
|RGB2HSV( ).S|Number|Saturation (0-255)|
|RGB2HSV( ).V|Number|Brightness value (0-255)|


<br/>

## HSV2RGB
Inverse conversion of *RGB2HSV*.

### Syntax

**HSV2RGB**( *Hue*, *Saturation*, *value* )

- Hue - Required. Hue value (0-360).
- Saturation - Required. Saturation (0-255).
- value - Required. Brightness value (0-255).

### Output

|Path|Type|Description|
|--|--|--|
|HSV2RGB( ).Color|Color|Color|
|HSV2RGB( ).R|Number|Red value|
|HSV2RGB( ).G|Number|Green value|
|HSV2RGB( ).B|Number|Blue value|

<br/>

## RGB2HSL
This converts RGB color to HSL.

### Syntax

**RGB2HSL**( *Red*, *Green*, *Blue* )

- Red - Required. Red value (0-255).
- Green - Required. Green value (0-255).
- Blue - Required. Blue value (0-255).

### Output

|Path|Type|Description|
|--|--|--|
|RGB2HSV( ).H|Number|Hue value (degree) (0-360)|
|RGB2HSV( ).S|Number|Saturation (0-255)|
|RGB2HSV( ).L|Number|Lightness (0-255)|


<br/>

## HSL2RGB
Inverse conversion of *RGB2HSL*.

### Syntax

**HSL2RGB**( *Hue*, *Saturation*, *Lightness* )

- Hue - Required. Hue value (0-360).
- Saturation - Required. Saturation (0-255).
- Lightness - Required. Lightness value (0-255).

### Output

|Path|Type|Description|
|--|--|--|
|HSL2RGB( ).Color|Color|Color|
|HSL2RGB( ).R|Number|Red value|
|HSL2RGB( ).G|Number|Green value|
|HSL2RGB( ).B|Number|Blue value|

# GeoUtils

Returns Distance/Angle between two separate locations.

## Distance
This returns distance between two locaitons in unit of meter.

### Syntax

**Distance**( *Lat1*, *Lng1*, *Lat1*, *Lng2* )

- Lat1 - Required. Latitude for location1.
- Lng1 - Required. Longitude for location1.
- Lat2 - Required. Latitude for location2.
- Lng2 - Required. Longitude for location2.


<br />

## BearingAngle
This returns bearing angle from location1 to location2.

(North: 0, East :90, South: 180, West: 270)

### Syntax

**BearningAngle**( *Lat1*, *Lng1*, *Lat1*, *Lng2* )

- Lat1 - Required. Latitude for location1.
- Lng1 - Required. Longitude for location1.
- Lat2 - Required. Latitude for location2.
- Lng2 - Required. Longitude for location2.


<br/>

# UnitCnvt

Unit converter for length, weight, and temperature.

## Length
Convert Length from specific unit to others

### Syntax

**Length**( *value*, *Unit*, *DecimalPoint* )

- value - Number : Required.
- Unit - Text : Required. Unit of input *value* (cm, m, km, inch, feet, mile)
- DecimalPoint - Number : Optional. Rounds converted value at given decimal point.

### Output
Type: Record.
Maker can access converted value by `UnitCnvt_1.Length(100,"m",2).inch` or so.

<br/>


## Weight
Convert Weight from specific unit to others

### Syntax

**Weight**( *value*, *Unit*, *DecimalPoint* )

- value - Number : Required.
- Unit - Text : Required. Unit of input *value* (g, kg, oz, lb)
- DecimalPoint - Number : Optional. Rounds converted value at given decimal point.

### Output
Same as Length
<br/>

## Temperature
Convert Temperature from specific unit to others

### Syntax

**Temperature**( *value*, *Unit*, *DecimalPoint* )

- value - Number : Required.
- Unit - Text : Required. Unit of input *value* (F, C, K)
- DecimalPoint - Number : Optional. Rounds converted value at given decimal point.

### Output
Same as Length

<br/>

# StatUtils

Statistics functions.

## MODE
Returns top N values in frequency order.

### Syntax

**MODE**( *InputTable*, *top* )

- InputTable - Table : Required. The column name should be `Value` and each value is Number-type. (e.g. `Table({Value:1},...,{Value:2})` or `[3,4,....,13]`)
- top - Number (Positive integer) : Required. 

### Output
Table with columns "value" and "freq".

## sMODE
Returns top N values in frequency order. (For String array)

### Syntax

**MODE**( *InputTable*, *top* )

- InputTable - Table : Required. The column name should be `Value` and each value is Text-type. (e.g. `Table({Value:"aaa"},...,{Value:"fff"})` or `["aaa",..,"fff"]`)
- top - Number (Positive integer) : Required. 

### Output
Table with columns "value" and "freq".

## Median
Returns the median of the given numbers. The median is the number in the middle of a set of numbers.

### Syntax

**Median**( *InputTable*)

- InputTable - Table : Required. The column name should be `Value` and each value is Number-type. (e.g. `Table({Value:1},...,{Value:2})` or `[4,...,8]`)

### Output
Number ( in the middle of a set of numbers).

## Histogram
Returns histogram in given Bin range.

**Histogram**( *DataTable*, *start*, *step*, *count* )

- DataTable - Table : Required. The column name should be `data` and each value is Number-type.
- start - Number : Required. Lower value of first bin.
- step - Number : Required. Gap between each bin.
- count - Number : Required. Count of bins.


### Output
Table with columns "data" and "freq".

<br/>

# MathUtils

## RANDARRAY
Returns random number array.

### Syntax

**RANDARRAY**( *rows*, *min*, *max*, *IsInteger* )

- rows - Number : Required. Length of array.
- min - Number : Required. 
- max - Number : Required.
- IsInteger - Boolean : Optional. If *true*, function returns random integer numbers.

### Output
Table with columns "Value".
<br/>

## RandPwd
Generates random password string with user specified condition.

### Syntax

**RandPwd**( *Uppercase*, *Lowercase*, *Number*, *Symbol*, *PasswordLength*, *AllowedSymbols* )

- Uppercase - Boolean : Required.
- Lowercase - Boolean : Required.
- Number - Boolean : Required.
- Symbol - Boolean : Required.
- PasswordLength - Number : Required.
- AllowedSymbols - Text : Optional. Allowed symbols (e.g. `![]$@()./`)

### Output
Random Password text.

