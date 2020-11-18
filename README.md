# SeeLab

### SeeLab - Processing for CIE spacess from sRGB - Beta 0.98

This object and methods parse sRGB color values, provide returns as strings, arrays, or numeric values, and process color data into and out of CIE standard spaces XYZ, xyY, LAB, LUV, LChab, LChuv, and a few other nifty things.

This project is an offshoot of the SAPC/APCA contrast project. This started as the sRGB input form, but has grown to include a number of useful methods including CIE processing, so I've made this a stand-alone library.

The "style.css" is for the color listing functions that list HTML color names with examples, and LUV colors, etc.

### Usage Examples

    var myColor = new RGBcolor(colorString)

Send a color string to RGBcolor for parsing, then:

`myColor.r` is an 8bit int of the red channel (.g for green and .b for blue)

`myColor.ok` is a boolean that returns true only if the colorString was successfully parsed.

`myColor.hex()` is a hex string of the RGB or RGBA (auto detects if alpha is present)

`myColor.CIE()` returns an array with CIE spaces XYZ, xyY, LAB, LCh, etc.


Copyright © 2019-2020 by Andrew Somers. All Rights Reserved.
LICENSE: GNU AGPL v3  https://www.gnu.org/licenses/
CONTACT: Please use the ISSUES tab at: https://github.com/Myndex/SeeLab/
