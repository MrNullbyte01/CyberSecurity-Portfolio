# NULL Motherboard

> A custom Raspberry Pi Zero 2 W carrier / motherboard designed in KiCad 10.

**Status: Design in progress — not fabricated or assembled.**

This repository section tracks the design of a custom carrier PCB for the Raspberry Pi Zero 2 W. The Raspberry Pi is the compute module; this project is the supporting PCB that will expose selected interfaces, provide connectors, and organise power and expansion connections.

## Project goals

- Design a clean, documented carrier PCB around the Raspberry Pi Zero 2 W.
- Provide deliberate access to selected GPIO and peripheral interfaces.
- Plan power input, distribution, protection, and connector placement before routing.
- Make the board understandable and maintainable through a complete KiCad schematic, PCB layout, BOM, and fabrication outputs.
- Validate the design before ordering or assembling a physical board.

## Target platform

The Raspberry Pi Zero 2 W is a 65 mm × 30 mm board with a 1 GHz quad-core 64-bit Arm Cortex-A53 processor, 512 MB RAM, 2.4 GHz Wi-Fi, Bluetooth 4.2, a 40-pin GPIO footprint, micro-USB power, USB OTG, mini-HDMI, microSD, and a CSI camera connector.

Official references:
- [Raspberry Pi Zero models and documentation](https://www.raspberrypi.com/documentation/computers/zero.html)
- [Raspberry Pi Zero 2 W product brief](https://datasheets.raspberrypi.com/rpizero2/raspberry-pi-zero-2-w-product-brief.pdf)
- [Raspberry Pi Zero 2 W reduced schematics](https://datasheets.raspberrypi.com/rpizero2/raspberry-pi-zero-2-w-reduced-schematics.pdf)
- [Raspberry Pi hardware and power documentation](https://www.raspberrypi.com/documentation/computers/raspberry-pi.html)

The official documentation must be treated as the source of truth for connector dimensions, pin functions, power limits, and reserved signals. In particular, do not assume that every GPIO pin is safe for arbitrary voltage or current.

## Current project state

| Area | Status | Notes |
|---|---|---|
| Platform selection | Selected | Raspberry Pi Zero 2 W |
| KiCad project setup | In progress | KiCad 10 |
| Functional block definition | Pending | Finalise the exact connector and expansion list |
| Power architecture | Pending | Input source, protection, regulation, current budget |
| GPIO mapping | Pending | Verify every signal against official documentation |
| Schematic | Not completed | Must describe the new carrier board, not the archived front panel |
| PCB placement and routing | Not completed | Depends on schematic and mechanical decisions |
| ERC / DRC | Pending | Run and review reports after design changes |
| BOM and fabrication files | Pending | Generate only after design validation |
| Physical fabrication / testing | Not started | No assembled motherboard is being claimed |

## Important file-history note

The files currently named `assets/Null Motherboard.kicad_sch`, `assets/Null Motherboard.kicad_pcb`, and `assets/Null Motherboard.kicad_pro` in the parent portfolio are an **older Front Panel PCB design**. They contain a 2×5 connector, two LEDs, and two push buttons. They are archived reference material and are **not** the new Raspberry Pi Zero 2 W carrier design.

The Front Panel design must remain separate. Do not use its DRC result as evidence that the new motherboard is electrically or mechanically validated.

## Design decisions to settle

1. **Power input:** choose the input connector and source; calculate the load budget for the Pi and all planned peripherals.
2. **Power protection:** define reverse-polarity, over-current, transient, and decoupling requirements as appropriate to the selected input.
3. **Pi connection:** choose the mechanical/electrical connection method and verify pin numbering, board orientation, and mounting-hole clearances.
4. **USB:** decide whether to expose USB OTG through a connector, hub, or another supported arrangement. Check the Pi Zero 2 W USB topology and signal routing requirements.
5. **GPIO:** define only the GPIO signals actually needed; document voltage levels and reserved pins.
6. **Expansion:** decide whether to include UART, I²C, SPI, buttons, status LEDs, display, or sensor connectors.
7. **Mechanical layout:** confirm board outline, Pi placement, mounting holes, connector access, component heights, and enclosure constraints.

## Planned workflow

1. Requirements and block diagram.
2. Datasheet review and pin / connector mapping.
3. Power architecture and calculations.
4. KiCad schematic capture.
5. ERC review and correction.
6. PCB outline, mounting, and component placement.
7. Routing, ground strategy, and design-rule setup.
8. DRC review and correction.
9. BOM, Gerbers, drill files, and fabrication review.
10. Physical assembly, first-power checks, and functional tests.

## Validation checklist

- [ ] Pi Zero 2 W mechanical drawing checked against the footprint and mounting holes.
- [ ] Connector orientation and pin numbering independently checked.
- [ ] Power input and regulator ratings verified against the calculated load.
- [ ] No GPIO signal exceeds the Pi's permitted voltage levels.
- [ ] USB and other high-speed signals follow the applicable design guidance.
- [ ] ERC has no unresolved errors; warnings are reviewed and documented.
- [ ] DRC has no unresolved errors; warnings are reviewed and documented.
- [ ] BOM and footprints match the intended parts.
- [ ] Gerber and drill outputs inspected in a viewer.
- [ ] First-power and functional test plan written before assembly.

## Safety and project integrity

This is an educational hardware design. A clean ERC or DRC report does not prove that a board is electrically safe or will work. Power calculations, schematic review, footprint verification, fabrication checks, and cautious first-power testing are still required.

Only mark a milestone complete after the corresponding work and evidence exist. The board is currently a design project; it has not been fabricated or tested.
