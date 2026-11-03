# Requirements & Constraints

Targets are proposed, not achieved.

| ID | Requirement | Verification |
|---|---|---|
| R1 | MQ-2/MQ-6 inputs stay within ESP32 ADC limits | Measure module AO and conditioned pin voltage |
| R2 | Flame input polarity is known | Safe electrical stimulus |
| R3 | DHT11 ambient data is read | Compare with reference instrument |
| R4 | OLED shows readings and system state | Visual inspection/serial log |
| R5 | Configured hazard input causes ALERT state | Inject safe test signal |
| R6 | Fan follows approved state logic | Measure driver output and fan current |
| R7 | Sensor disconnect is handled safely | Controlled fault injection |
| R8 | Local operation works without Wi-Fi | Disable Wi-Fi and repeat tests |

Never mark a test passed without evidence. ESP32 GPIO is 3.3 V; MQ raw ADC values are not ppm. Keep all tests low-voltage DC.