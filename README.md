# Gcode-Pause-Print
Gcode to pause print and lift print head


```
G91 ; Set to relative positioning mode
G1 Z70 ; Move the print head up by 10 mm relative to the current position
M25 ; Pause the print
G1 Z-70 ; Move the print head down by 10 mm relative to the current position
G90 ; Set back to absolute positioning mode
```
