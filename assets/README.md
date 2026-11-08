# Portfolio Asset Index

This folder contains portfolio-level assets such as the profile photo, education/certificate material, and historical project evidence. Project-specific working files are organised in their dedicated repositories.

## Project assets copied to dedicated repositories

| Original asset group | Dedicated repository | Destination |
|---|---|---|
| Cisco Packet Tracer topology screenshots | [Cisco Networking Labs](https://github.com/MrNullbyte01/Cisco-Networking-Labs) | `evidence/` |
| Legacy KiCad Front Panel project and image | [NULL Motherboard](https://github.com/MrNullbyte01/NULL-Motherboard) | `archive/front-panel-reference/` |
| CTF and technical study PDFs | [CTF Writeups](https://github.com/MrNullbyte01/CTF-Writeups) | `writeups/` |

The original Packet Tracer and CTF source copies remain here. The duplicate Front Panel KiCad files and image were removed from this folder after their SHA hashes were verified against the archived copies in the NULL Motherboard repository.

## Assets that stay in the portfolio

- `profile-photo.jpeg` — used by the portfolio website.
- Texnoera diploma image/PDF — education/credential material, not a project asset.
- Other personal portfolio presentation assets.

## Assets not duplicated

- BlackBerry APK and BAR packages remain in the original `projects/blackberry-passport/` archive. They appear to include third-party application binaries; redistribution rights have not been verified. Their inventory is documented in the [BlackBerry Passport Revival repository](https://github.com/MrNullbyte01/BlackBerry-Passport-Revival/blob/main/docs/software-inventory.md).
- No personal Raspberry Pi Cyberdeck build photos or wiring diagrams were present in the portfolio assets at the time of review. The Cyberdeck repository separately contains 10 STL model files and reference research; their presence does not prove a physical assembly.

## Important NULL Motherboard distinction

The KiCad files formerly named `Null Motherboard.*` are the archived **Front Panel PCB**, not the new Raspberry Pi Zero 2 W carrier/motherboard. They have been renamed and placed under `archive/front-panel-reference/` in the NULL Motherboard repository to avoid confusion.
