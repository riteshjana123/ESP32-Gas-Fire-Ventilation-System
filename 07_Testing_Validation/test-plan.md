# Test Plan

| ID | Test | Method | Evidence |
|---|---|---|---|
| T1 | Power integrity | Measure rails idle/fan start | DMM readings |
| T2 | ADC safety | Measure raw AO and conditioned pin | Voltage table |
| T3 | Sensor baseline | Datasheet warm-up and log | Serial CSV |
| T4 | Flame input | Safe electrical stimulus | Logic table |
| T5 | Alarm state | Inject simulated hazard | Log/video |
| T6 | Fan actuation | Low-voltage driver test | Current/voltage/photo |
| T7 | Sensor fault | Controlled disconnect | Fault log |
| T8 | Offline behaviour | Disable Wi-Fi | Test log |

Do not release LPG, create smoke or use open flame for testing.