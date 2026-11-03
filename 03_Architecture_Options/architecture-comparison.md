# Architecture Options

**A — Single ESP32:** all sensing, state logic, OLED and actuator control on one MCU. Lowest complexity; shared controller/power fault is a limitation. Recommended first build.

**B — ESP32 + conditioned analog front end:** add divider, filtering and protection for MQ analog outputs. Better signal integrity/testability; more parts. Adopt the protection elements from this option in the selected design.

**C — Distributed wireless nodes:** modular but adds communication failure modes and complexity. Not recommended for the first demonstrator.

**Selection:** Option A with appropriate input conditioning from B. Local alarm/control must never depend on Wi-Fi.

**Block flow:** MQ-2/MQ-6 → conditioning → ESP32 ADC; flame module → verified GPIO; DHT11 → GPIO; ESP32 → OLED; ESP32 → low-voltage fan driver and alarm.