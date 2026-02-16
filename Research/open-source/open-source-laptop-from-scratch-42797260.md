---
title: "Show HN: I made an open-source laptop from scratch"
url: "https://www.byran.ee/posts/creation/"
hn_id: "42797260"
hn_url: "https://news.ycombinator.com/item?id=42797260"
date: 2026-02-16
topic: "open source"
tags: [research, open-source, hardware, laptop, diy]
source: hackernews
points: 3237
---

# Summary

A developer named Byran spent approximately six months engineering a fully open-source laptop from scratch. The project demonstrates that individuals can build sophisticated hardware with modern features including a 4K AMOLED display, Cherry MX mechanical keyboard, capability to play Minecraft at 4K, run 7B+ parameter LLMs locally, and achieve approximately 7 hours of battery life.

The laptop is built around the Rockchip RK3588 SoC using a FriendlyElec CM3588 System on Module (SoM). The hardware design includes a custom motherboard with dual USB 3.1 Type-C ports, USB 2.0 Type-A, headphone jack, and microSD card slot. The display is a Samsung ATNA33TP11 4K AMOLED panel, which required significant reverse-engineering work to get running on Linux.

The powertrain features a custom design with an ESP32-S3 embedded controller managing a ~60Wh lithium-ion battery pack. The keyboard is a wireless mechanical design using Cherry MX ULP switches running ZMK firmware on an nRF52840 SoC. All schematics, CAD files, and design documentation are available on GitHub under open-source licenses.

The project serves as a practical demonstration that open-source hardware can achieve commercial-grade results. It also provides detailed documentation for others who want to learn about laptop design, including system integration, power management, display interfacing, and peripheral development.

## Key Points
- Full laptop built from scratch with RK3588 SoC and 4K AMOLED display
- ~7 hour battery life with custom 60Wh battery management system
- Cherry MX mechanical keyboard with wireless ZMK firmware
- All schematics and CAD files available on GitHub
- Capable of running modern workloads including LLMs and games

## Relevance to open source
This project exemplifies the potential of open-source hardware development. By releasing all design files, schematics, and firmware openly, the creator enables others to learn, modify, and build upon the work. It challenges the notion that only large corporations can produce sophisticated consumer electronics.
