# Journal




## 21 Oct 2026 - 12:19 to 14:46 (2h 27m)
- I set up the repo and journal and 
- found the ATtiny412 on mouser and checked the pinout in the datasheet
- started the schematic:
  - ATtiny412 with a cap and UPDI header
  - MCP23017 wired up with pull ups
  - both RJ45 jacks wired to the MCP23017
  - 8 WS2812B leds chained together
- fixed a few mistakes like caps in the wrong place, power pins backwards, labels swapped
- next: button, debug header and usb-c

## 5 Nov 2026, 13:56 to 14:59 (1 h 3m)
- set up the repo and journal
- added the test button
- added a debug header for serial
- added usb-c power with the 5.1k resistors
- added power flags to fix ERC errors
- ERC passes with 0 errors, schematic done
- next: pick the parts on mouser and assign footprints

## 9 Nov 2026 - 10:11 to 12:27 (2h 16m)
- picked parts for every part of the board and added part numbers in kicad
- mouser doesn't sell bare WS2812B LEDs, so I looked at an 8mm through hole one but found two different pinouts online so went with 5050 smd ones from digikey (Inolux IN-PI55TATPRPGPB)
- picked a cheap Amphenol RJ45 jack (54602-908LF) that already has a kicad footprint
- picked a GCT USB4125-GF-A for usb-c power, also has a kicad footprint
- changed the debug header to 3 pins (TX, GND, 5V) so both headers are the same part
- parts for one board come to about £8.50
- next: check the LED pinout, change C3 to a polarised cap, assign footprints
