# Firmware

Firmware will be added after schematic and GPIO map are confirmed. Planned modules: main loop; sensor acquisition/validation; safety state machine with hysteresis; OLED; actuator control. Keep loop non-blocking. Do not freeze GPIO assignments until ADC-capable pins, active levels, scaling and safe output defaults are verified.