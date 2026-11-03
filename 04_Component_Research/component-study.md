# Component Research

| Part | Role | Checks |
|---|---|---|
| ESP32 DevKit V1 | Controller | Exact pinout, ADC pins/range, boot pins |
| MQ-2 / MQ-6 | Gas/smoke response | Heater current, AO maximum, DO polarity, warm-up, datasheet |
| Flame module | Flame indication | Supply, output type/polarity/voltage, IR interference |
| DHT11 | Ambient context | Supply, pull-up, accuracy/response limits |
| I2C OLED | Display | Controller, address, logic voltage, pull-ups |
| Relay/driver | Fan switching | 3.3 V input compatibility, coil/contact ratings |
| 5 V fan | Ventilation demo | Rated/startup current, polarity, transient handling |

MQ readings drift with environment and ageing. Do not claim ppm without a defensible calibration method.