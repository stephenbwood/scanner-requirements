# SCANNER REQUIREMENTS

## CONFIGURATION
Operator adjustable values should be available through a standard configuration file.

## EXPOSURE MODES
* **Variable**
  Uses a floating exposure and color correction values to maintain average brightness and white balance.
* **Variable with Lock**
  Same as Variable, but with the option to hold the current exposure/backlight correction values until unlocked.
* **Stepped Variable**
  Uses predefined set of exposure/color correction values with corresponding minimum and/or maximum threshold values.
* **Manual**
  Operator defined exposure / color correction.

## FILE OUTPUT
* Camera RAW (IIQ)
* TIFF 8-bit / 16-bit
* JPEG

## OUTPUT LOCATION
The output location for captured files should be defined through the configuration file.

## NAMING CONVENTIONS
File names should reflect the current order, roll, and frame in the format:`{Order}_{Roll}_{Frame}`

**Acquiring Order Id**

The value for `{Order}` should be user input.

**Acquiring Roll Id**

The value for `{Roll}` should be user input.

**Acquiring Frame Id**

The value for `{Frame}` should depend on the film format.

| Format | Acquisition |
| ------ | ----------- |
| 135 | DX-Code |
| 120 / 220 | Auto-incrementing from 1 |
