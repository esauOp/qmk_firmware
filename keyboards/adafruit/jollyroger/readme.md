# Handwired macropad based on Adafruit MacroPad RP2040

A RP2040-powered Macropad with a 3x2 layout.

- Keyboard Maintainer: 
- Hardware Supported: Raspberry Pi Pico / RP2040
- Hardware Availability:

Make example for this board (after setting up your build environment):

```sh
qmk compile -kb adafruit/jollyroger -km default
```

See the [build environment setup](https://docs.qmk.fm/#/getting_started_build_tools) and the [make instructions](https://docs.qmk.fm/#/getting_started_make_guide) for more information. Brand new to QMK? Start with our [Complete Newbs Guide](https://docs.qmk.fm/#/newbs).

## Features

- Raspberry Pi RP2040 Chip + 8MB Flash memory - Dual-core Cortex M0+ at ~130MHz with 264KB of RAM.
- 3x2 Mechanical key switch sockets - accepts any Cherry MX-compatible switches. Individually tied to GPIO pins (not matrix wired)
- 6x NeoPixel RGB LED.
- Rotary encoder, 20 detents per rotation, with push-switch on GPIO pin.

## Bootloader

Enter the bootloader in 4 ways:

* **Bootmagic reset**: Hold down the key just below the rotary encoder push-button on power-up.
* **BOOT button** Hold down the rotary encoder push-button on power-up or reset.
* **Keycode in layout**: Press the key mapped to `QK_BOOT` if it is available.
