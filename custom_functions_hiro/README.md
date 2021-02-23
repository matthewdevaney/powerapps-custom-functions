# List of components in my library

- [ColorUtils](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_hiro#colorutils)
- [GeoUtils](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_hiro#geoutils)
- [UnitCnvt](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_hiro#unitcnvt)


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
Length() returns Table.
User can get converted value by using LookUp function.

Example of response:

```json
[
  {
    "unit": "cm",
    "value": 2000
  },
  {
    "unit": "m",
    "value": 20
  },
  {
    "unit": "km",
    "value": 0.02
  },
  {
    "unit": "inch",
    "value": 787.4015748031496
  },
  {
    "unit": "feet",
    "value": 65.61679790026247
  },
  {
    "unit": "yard",
    "value": 21.872265966754156
  },
  {
    "unit": "mile",
    "value": 0.012427454732996135
  }
]
```
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
