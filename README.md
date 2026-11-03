# ESP32 Gas & Fire Detection with Automatic Ventilation

Educational ESP32 prototype for gas/smoke sensing, flame indication, local alarm logic and low-voltage ventilation control.

> **Safety:** This is not a certified gas detector, fire alarm, or life-safety device. Do not release LPG, create smoke, use open flame, or switch mains loads during testing. Use supervised low-voltage bench tests only.

## Status
Engineering design foundation. Measurements, photos, simulations and test results are pending and will be added only after they are genuinely produced.

## Planned hardware
ESP32 DevKit V1, MQ-2, MQ-6, flame sensor, DHT11, 0.96-inch I2C OLED, low-voltage relay/driver and 5 V fan. Verify exact module variants and electrical ratings before connection.

## Key engineering constraints
- ESP32 GPIO is 3.3 V: never connect 5 V sensor AO/DO directly.
- Measure MQ module output voltage and condition it before ADC connection.
- MQ raw ADC values are not ppm; warm-up and calibration are required.
- Verify fan startup current, driver/relay compatibility and supply capacity.
- Keep local alarm/control independent of Wi-Fi.
- Record real measurements and failures; never fabricate evidence.

## Assessment folders
01_Problem_Opportunity; 02_Requirements; 03_Architecture_Options; 04_Component_Research; 05_Design_Files; 06_Prototype_Build; 07_Testing_Validation; 08_Iteration_Improvements; 09_Evidence; 10_BOM_References; 11_Final_Report; 12_Declaration; firmware.

Prior related work: [LPG-Security-System](https://github.com/riteshjana123/LPG-Security-System). Its previous photos/results are not evidence for this assessment.