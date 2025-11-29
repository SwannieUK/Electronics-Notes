Removing electronics from from case
- Use a spudger to pop the glued side tabs, approx. the middle
- Remove mouthpiece by snapping off
- Remove slider switch from bottom
- Ease the internals out of the body - they will all come out - be careful at the top as the pcb is there. be careful ~1/4 up from the bottom as the LIon cell is there. 
- Optionally pop off of screen and button from the PCB
- Remove microphone from plastic base
- Cut heating element wires
- Remove from juice tank, discard juice tank
- Remove padding from ends of cell

Internals
- 3.7V 850mAh R17350D (17x35mm) - 3.15Wh
- Microphone - 3 wire
- CH6057 charge controller IC
- USBC port
- sliders switch - SP4T? - does not isolate usb or cell
- TM52F1376 MCU
- Button
- 19 segment LCD with back light
  - TURBO x 1
  - III x 3
  - "ice" x 4
  - "bars" x 1
  - "battery" x 5
  - "juice" x 5
- 3x heating elements
  - 2x in tank 1
  - 1x in tank 2

PCB
- C3 is missing... Remove after programming?

USB
- Not standard
- SWDIO and SWCLK connected to pins
- IO and CLK match with D and C on 4pin header VDCG
- D and C match to pin 28 and 27 on MCU: likely PSDA and PSCL for vendor programmer, optional UART TXD/RXD
  - Attempted to find I2C address on these pins, but doesn't appear to be found