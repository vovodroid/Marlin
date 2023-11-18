# BIQU B1 SE (SKR 2) Firmware

Flash drive support is enabled, but jumpers to enable support may not have been installed correctly from the factory. [Follow Biqu's instructions, starting with Step 2](https://github.com/bigtreetech/BIQU-B1-SE-PLUS/blob/master/B1-SE%20fimware/B1-SE-U%20Disk%20Usage%20Tutorial-English.pdf) if flash drive support is not working correctly.

M503 report from original B1 SE BTT firmware:
```
echo:  G21    ; Units in mm (mm)

echo:; Filament settings: Disabled
echo:  M200 S0 D1.75
echo:; Steps per unit:
echo: M92 X80.00 Y80.00 Z400.00 E92.00
echo:; Maximum feedrates (units/s):
echo:  M203 X150.00 Y150.00 Z5.00 E65.00
echo:; Maximum Acceleration (units/s2):
echo:  M201 X1000.00 Y1000.00 Z100.00 E10000.00
echo:; Acceleration (units/s2): P<print_accel> R<retract_accel> T<travel_accel>
echo:  M204 P500.00 R500.00 T500.00
echo:; Advanced: B<min_segment_time_us> S<min_feedrate> T<min_travel_feedrate> J<junc_dev>
echo:  M205 B20000.00 S0.00 T0.00 J0.01
echo:; Home offset:
echo:  M206 X0.00 Y0.00 Z0.00
echo:; PID settings:
echo:  M301 P19.32 I1.32 D70.43
echo:  M304 P41.78 I7.32 D158.93
; Controller Fan
echo:  M710 S255 I0 A1 D60 ; (100% 0%)
echo:; Power-Loss Recovery:
echo:  M413 S1
echo:; Z-Probe Offset (mm):
echo:  M851 X0.00 Y0.00 Z0.20
echo:; Stepper driver current:
echo:  M906 X800 Y800 Z800
echo:  M906 T0 E800

echo:; Driver stepping mode:
echo:  M569 S1 X Y Z
echo:  M569 S1 T0 E
echo:; Filament load/unload lengths:
echo:  M603 L0.00 U100.00
echo:; Filament runout sensor:
echo:  M412 S0
echo:; Babystep total:
echo:  M290 Z0
```
