# Scanner Requirements

## Configuration
Operator adjustable values should be available through a standard configuration file.

## Exposure Modes
* **Variable**
  Uses a floating exposure and color correction values to maintain average brightness and white balance.
* **Variable with Lock**
  Same as Variable, but with the option to hold the current exposure/backlight correction values until unlocked.
* **Stepped Variable**
  Uses predefined set of exposure/color correction values with corresponding minimum and/or maximum threshold values.
* **Manual**
  Operator defined exposure / color correction.

## Output File Types
* Camera RAW (IIQ)
* TIFF 8-bit / 16-bit
* JPEG

## Output Location
The output location for captured files should be defined through the configuration file.

## Naming Conventions
File names should reflect the current order, roll, and frame in the format:`{Order}_{Roll}_{Frame}`

### Acquiring Order Id
The value for `{Order}` should be user input.

### Acquiring Roll Id
The value for `{Roll}` should be user input.

### Acquiring Frame Id
The value for `{Frame}` should depend on the film format.

| Format | Acquisition |
| ------ | ----------- |
| 135 | DX-Code |
| 120 / 220 | Auto-incrementing from 1 |

## Dust & Scratch Removal
The scanner should have dust and scratch removal based on the infrared sensitivity of the imaging sensor.
