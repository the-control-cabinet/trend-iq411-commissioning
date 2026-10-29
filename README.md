# Trend IQ411 Commissioning: Real DDC on the Training Rig (Planned)

**Putting a real Trend IQ411 controller (a widely used UK BMS outstation) onto the training rig: power-up and addressing, I/O commissioning, writing strategy in Trend's System Engineering Tool (SET), then re-implementing the rig's duty/standby, interlock and PID sequences in Trend strategy and comparing them with the ESP32 versions. The aim is hands-on Trend experience, not just theory.**

[![YouTube](https://img.shields.io/badge/YouTube-The%20Control%20Cabinet-red?logo=youtube)](https://www.youtube.com/channel/UC5Cupmz7vlfcodpCX7k8iuQ)
[![Portfolio](https://img.shields.io/badge/Portfolio-the--control--cabinet-24292f?logo=github)](https://github.com/the-control-cabinet/the-control-cabinet)
![Domain](https://img.shields.io/badge/BMS-Trend%20IQ4-blue)
![Status](https://img.shields.io/badge/Status-Planned-yellow)

> **The short version:**
> - **Hardware:** a Trend IQ411 (230 V mains variant) on row 1 of the DIN-rail rig, on its own MCB.
> - **Commissioning:** power, addressing, comms to SET ⟨connection method to confirm for this model⟩, then I/O point-to-point checks.
> - **Strategy:** duty/standby (#7), interlocks (#9) and a PID loop (#8) written in Trend strategy modules: sensors, knobs, switches, loops, logic, drivers, time zones.
> - **Comparison:** the same sequences on ESP32/ESPHome vs Trend: engineering effort, behaviour, diagnostics.

**Portfolio position:** Field/automation level · vendor DDC (portfolio #12). PLC counterpart: [PLC re-implementation](https://github.com/the-control-cabinet/plc-reimplementation-iec61131) (#13). Rig companions: [duty/standby + interlocks](https://github.com/the-control-cabinet/din-rail-rig-duty-standby-interlocks) · [PID rig](https://github.com/the-control-cabinet/pid-anti-hunt-control-rig)

---

## Documents

| Doc | Contents |
|---|---|
| [01 Hardware and comms](docs/01-hardware-and-comms.md) | Power, addressing, SET connection, I/O schedule |
| [02 Commissioning procedure](docs/02-commissioning.md) | Point-to-point checks, strategy download, functional tests |
| [03 Strategy design](docs/03-strategy.md) | Duty/standby, interlocks and PID in Trend modules |

## Roadmap
- [ ] Record the IQ411 I/O and comms details from the datasheet
- [ ] Source or confirm SET access
- [ ] Power up, address and connect
- [ ] Point-to-point I/O commissioning
- [ ] Strategy: duty/standby → interlocks → PID
- [ ] Comparison write-up vs ESP32

## Skills demonstrated (as built)
| Skill | Evidence |
|---|---|
| Vendor DDC | Trend IQ411 hands-on |
| Commissioning | Point-to-point I/O, strategy download, functional tests |
| Trend strategy | Sensors, knobs, switches, loops, logic, drivers, time zones |
| Platform comparison | Same sequences on ESPHome vs Trend |

📺 [The Control Cabinet on YouTube](https://www.youtube.com/channel/UC5Cupmz7vlfcodpCX7k8iuQ)

*Built and documented by James · part of [The Control Cabinet BMS portfolio](https://github.com/the-control-cabinet/the-control-cabinet). MIT Licence.*
