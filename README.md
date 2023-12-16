# Gcode-Pause-Print
This is Gcode that i use to interrupt the print with PrusaSlicer. 
It will lift the head bei 70mm in Z. So you can easily do filament color changes during print. 

Works with Octroprint & Ender 3 V2 (Standard Firmware)


```
G91 ; Set to relative positioning mode
G1 Z70 ; Move the print head up by 10 mm relative to the current position
M25 ; Pause the print
G1 Z-70 ; Move the print head down by 10 mm relative to the current position
G90 ; Set back to absolute positioning mode
M83; to not set Extruder to absolute
```
