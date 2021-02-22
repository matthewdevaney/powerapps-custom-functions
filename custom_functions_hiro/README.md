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
