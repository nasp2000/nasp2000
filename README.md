<div align="center">

# Nuno Pereira

**Desktop software in Rust, firmware for ESP32, and small web tools.**
Old ideas, modern hardware.

**I am not a programmer and I have no intention of becoming one. I am a human
full of ideas — ~99% of the code here is executed by AI.**

📍 Arraiolos, Portugal

[![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)](#)
[![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white)](#)
[![ESP32](https://img.shields.io/badge/ESP32--S3%20%2F%20P4-E7352C?style=flat-square&logo=espressif&logoColor=white)](#)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](#)
[![License](https://img.shields.io/badge/license-MIT%20%2F%20Apache--2.0-3DA639?style=flat-square)](#)

</div>

---

## What I'm working on

Two projects take almost all of my time today: **Node32-HUB** and **BeamBurin**.

### [Node32-HUB](https://github.com/nasp2000/Node32-HUB) — main project
One modular firmware framework for ESP32-S3 and ESP32-P4: RS232, LPT/DB25, Modbus
RTU/TCP, CAN, GRBL, sensors, email, scheduler, camera, radio and audio, over Wi-Fi
or wired Ethernet. Compile-time feature flags ("packs") turn the same codebase into
completely different devices — disabled modules cost zero RAM. Around it sits a
whole family of firmwares built from the same code: Node32-OEE, Rambox32, Cam-M,
GcodeSender, Harmonica-BOX and the WebSerial flasher.

### [BeamBurin](https://github.com/nasp2000/BeamBurin) — main project
Vector drawing and job preparation for laser engraving and cutting. Draw, import
SVG/DXF/HPGL/PDF, assign operations to layers with speed, power, passes, kerf and
tabs, preview and estimate, then export the job file to the sender of your choice.
Portable, offline, and it deliberately **never controls a machine**.

### [FreePlots](https://github.com/nasp2000/FreePlots) — also in the workshop
Classic industrial statistics, rebuilt as a free desktop application in Rust.
Worksheet + Session report, descriptive statistics, capability, control charts, MSA,
hypothesis tests, ANOVA, regression, DOE and reliability — offline, MIT, one
executable, no account and no telemetry. Every report states its method, sample
size, exclusions and warnings instead of hiding them behind a number.

---

## Projects

| Project | What it is | Stack |
| --- | --- | --- |
| ⭐ [Node32-HUB](https://github.com/nasp2000/Node32-HUB) | **Main project** — modular multi-protocol ESP32 firmware framework | C++ · ESP-IDF |
| ⭐ [BeamBurin](https://github.com/nasp2000/BeamBurin) | **Main project** — laser engraving / cutting job editor and preparation tool | Rust |
| [FreePlots](https://github.com/nasp2000/FreePlots) | Statistics and quality-analysis desktop app (SPC, MSA, DOE, reliability) | Rust · egui |
| [Node32-OEE](https://github.com/nasp2000/Node32-OEE) | Industrial OEE and production counting firmware (AxPxQ, shifts, CSV, email) | C++ · ESP32 |
| [Rambox32](https://github.com/nasp2000/Rambox32) | Pigeon-racing timing terminal: RS232 + Unikon, OLED, email alerts, OTA | C++ · ESP32 |
| [GcodeSender](https://github.com/nasp2000/GcodeSender) | Standalone G-code sender over USB Host with a local web UI | C++ · ESP32 |
| [Cam-M](https://github.com/nasp2000/Cam-M) | Camera companion firmware: MJPEG stream, snapshots, AVI, motion detection | C++ · ESP32 |
| [Harmonica-BOX](https://github.com/nasp2000/Harmonica-BOX) | Internet-radio streaming firmware | C++ · ESP32 |
| [Edit.GC](https://github.com/nasp2000/Edit.GC) | Browser-based G-code editor with a visual toolpath and point editor | JavaScript |
| [webflasher_Node32-HUB](https://github.com/nasp2000/webflasher_Node32-HUB) | WebSerial flasher and Wi-Fi configurator — no Python, no esptool | HTML · JS |
| [LPT-UNO](https://github.com/nasp2000/LPT-UNO) | Parallel port (LPT/DB25) printer emulator on an Arduino Uno | C++ · Arduino |

---

## AI does the typing

I am not a programmer, and I do not intend to become one. I am a human full of
ideas, and every project here is **executed ~99% by AI**. Almost every line of
code, test, script and documentation page is written by an AI agent working inside
the repository; my job is the part that cannot be delegated:

- coming up with the idea in the first place, and deciding *what* gets built;
- writing the brief the agent works from, in plain language and in detail;
- reviewing what comes back, running it on real hardware, and rejecting it when it
  is wrong;
- keeping the rules that make AI output usable: tests first, docs in the same
  change, one version bump per release, nothing merged blind.

That is why these projects exist at all. A multi-board firmware framework and a
laser job editor are not one-person jobs — but one person with ideas and an AI that
does the typing can ship them. The discipline is what keeps them shippable.

## How I work

- **AI-written, human-judged.** No feature is accepted because "the model said so":
  it needs a written spec, a test that fails before it and passes after, and a doc
  update in the same change.
- **Tests are part of the build.** Native `doctest` suites, jsdom web tests, and
  hardware regression scripts that refuse to publish when a pack loses persistence.
- **Licensing is engineering, not paperwork.** Dependencies pinned to exact versions,
  an SBOM, third-party notices, and an LGPL bundle shipped with every build.
- **Docs live next to the code.** Architecture notes, pinouts, and a per-page
  document for every web screen — because "how it works" is part of the product.
- **Offline and portable by default.** No installers, no admin rights, no telemetry,
  no cloud dependency where a local program will do.

---

<div align="center">

![Nuno's GitHub stats](https://github-readme-stats.vercel.app/api?username=nasp2000&show_icons=true&hide_title=true&hide_rank=true&theme=transparent&border_color=30363d)

*It all comes down to time and what we do with it.*

</div>
