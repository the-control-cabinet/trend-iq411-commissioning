# 03 Strategy design

[← Back to README](../README.md)

| Function | Trend approach (planned) |
|---|---|
| Inputs | Sensor modules (scaling, alarm limits) |
| Setpoints / adjustments | Knob modules |
| Pump enables | Switch + logic modules; driver modules to outputs |
| Duty/standby | Logic for lead selection by run hours; failover on a proving input |
| Interlocks | Logic gating the drivers (permissives, latch for lockout) |
| PID | Loop module (proportional band, integral time; Trend's anti-windup behaviour to document) |
| Schedules | Time zone modules |

**Comparison:** the same sequences on ESPHome, Trend and an IEC 61131-3 PLC are compared side by side in the [PLC repo's three-platform comparison](https://github.com/the-control-cabinet/plc-reimplementation-iec61131/blob/main/docs/03-three-platform-comparison.md).
