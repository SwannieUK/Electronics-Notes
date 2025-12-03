## Device Information

"ESP32 C3 Development board desktop trinket Mini TV Portable Pendant LVGL 1.44inch LCD ST7735 LVGL Weather Station GIF Animation"

Product Docs: https://spotpear.com/wiki/ESP32-C3-desktop-trinket-Mini-TV-Portable-Pendant-LVGL-1.44inch-LCD-ST7735.html

Example App: https://github.com/Spotpear/ESP32C3_1.44inch

## Hardware
- Schematics: https://cdn.static.spotpear.com/uploads/picture/product/esp32/ESP32C3-1.44/Schematic/ESP32-C3-1.44inch.pdf

- No on/off switch - identify the best location to add a small SPST switch - on battery lead, or on the board - likely the lead.
- Backlight power - very bright - need to understand the schematics
  - Looks like the driver is ST7735 ?
  - Looks like Pin18 / IO11 goes to LED backlight - should be potential to PWM it.
- Single Core, therefore limited in things like presenting extra USB-HID.
  - Potentially pair with a RP2040, or similar?

## Software

- GhostESP Revival - "out of the box" for C3
  - no screen support
    - AWOK-Mini seems to have similar screen (dimensions, driver)
      - Look to create a new sdkconfig for this device.
      - https://github.com/jaylikesbunda/Ghost_ESP/blob/Development-deki/configs/sdkconfig.awokmini
- Bruce?
- Maurauder?
