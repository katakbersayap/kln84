# Klandestin84

Handwired RP2040 ortholinear84 Keyboard Project

## Keyboard Layout Preview

![Klandestin84](images/keyboard_layout_kln84.jpg)

## Keyboard Wiring Preview

![Klandestin84 Wiring](images/kln84_wiring.jpg)

## VIA Support

![Klandestin84 Via Support](images/via_support_kl84.jpg)

*A short description of the keyboard/project*

* Keyboard Maintainer: [Alif Faizin](https://github.com/katakbersayap)
* Hardware Supported: *Raspberry Pi Pico RP2040*
* Firmware: *QMK Firmware*
* Layout : *Custom (ortholinear / handwired)*

## Matrix Pins:

    "cols": ["GP6","GP7","GP8","GP9","GP10","GP11","GP12","GP13",
             "GP14","GP15","GP16","GP17","GP18","GP19","GP20"],
    
    "rows": ["GP0","GP1","GP2","GP3","GP4","GP5"]


## Flashing Firmware :
1. Compile firmware using QMK MSYS
2. Put RP2040 (Pi Pico) into bootloader mode
3. copy the generated `.uf2` file into the RP2040 (Pi Pico) drive

## Notes
* Ensure matrix wiring matches your QMK configuration
* Use the command : `qmk compile -kb <keyboard> -km default

See the [build environment setup](https://docs.qmk.fm/#/getting_started_build_tools) and the [make instructions](https://docs.qmk.fm/#/getting_started_make_guide) for more information. Brand new to QMK? Start with our [Complete Newbs Guide](https://docs.qmk.fm/#/newbs).

## Bootloader

Enter the bootloader in 3 ways:

* **Bootmagic reset**: Hold down the key at (0,0) in the matrix (usually the top left key or Escape) and plug in the keyboard
* **Physical reset button**: Briefly press the button on the back of the PCB - some may have pads you must short instead
* **Keycode in layout**: Press the key mapped to `QK_BOOT` if it is available
