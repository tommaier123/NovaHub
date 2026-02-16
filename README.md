# Nova Hub

This project aims to create a simple but small battery powered OpenShock hub.

<img src="https://github.com/tommaier123/NovaHub/blob/main/Pictures/Complete.jpg" height="330"/> <img src="https://github.com/tommaier123/NovaHub/blob/main/Pictures/Internal.jpg" height="330"/> <img src="https://github.com/tommaier123/NovaHub/blob/main/Pictures/Lid.jpg" height="330"/>

---

## Benefits
- No custom PCB necessary
- No external antenna necessary
- Small size 31x25x46mm
- Large capacity (1100mAh) should last for at least 12h

---

## Bill of Materials
- 1× Mini switch SS12D00 ~(3.7x3.7x8.7mm) with 3mm stem [AliExpress link](https://de.aliexpress.com/item/1005010427557422.html) or [Amazon DE link](https://www.amazon.de/-/en/dp/B09TVFF6KW)
- 1× Esp32 S3 SuperMini (must have battery charging) [AliExpress link](https://de.aliexpress.com/item/1005006583245248.html) or [AliExpress link](https://de.aliexpress.com/item/1005010580012002.html)
- 1× Opensmart 433MHz Transmitter [OpenShock Wiki](https://wiki.openshock.org/hardware/transmitter/china/open-smart)
- 1× Meshnology 1100mAh battery [Amazon DE link](https://www.amazon.de/Meshnology-USB-Ladekabel-102540-Schutzplatine-Isoliertes/dp/B0F1FJ238M?th=1) 

  Other 102540 batteries could work as an alternative (dimensions 10x25x40mm)

---

## Printed Parts
- Base, Lid and Spacer in PLA (light colored if you want to see the LEDs)
- (Optional) Stencil in black/dark PLA (will prevent light leak between the LEDs)

---

## Printing Tips
(Tested on Prusa Core One and Bambulab H2D)
- 0.4 mm nozzle
- 0.1 mm layer height
- 15% infill
- No supports

**Optional:**
- Satin or smooth build plate
---

## Assembly Instructions
1. (Optional) connect the bottom jumper of the SuperMini for faster charging (300mA instead of 100mA). **Be very careful the pads break of easily**

<img src="https://github.com/tommaier123/NovaHub/blob/main/Pictures/Board.jpg" height="200"/>

2. Install the battery at the bottom of the base
3. Solder wires to the Opensmart Transmitter
4. Place the Opensmart Transmitter on top of the shelf in the base walls
5. Install the Spacer with the open side facing the front (USB C port)
6. Remove the left or right most pin from the switch
7. Install the switch with some force. By choosing which way you install it you can select if left or right is on
8. Solder the battery positive to on of the switch pins and a wire to the other one
9. Solder the battery minus to the SuperMini battery minus pad (on the bottom) and the switch wire to the SuperMini battery plus pad (on the bottom)
10. Install the SuperMini in the Spacer
11. Solder the Opensmart Transmitter pins to the SuperMini (on the top). Connect GND to GND, VCC to 3.3V and SIG to pin 13
12. (Optional) install the black stencil on the lid (optionally glue it down)
13. Check that the OpenSmart board is all the way at the back, the spacer is all the way down and the SuperMini is seated flush
14. Download the firmware from the [Custom Boards Repository](https://github.com/tommaier123/Firmware/releases)

    There are two versions a default one that uses the RGB LED and one that uses the red LED
15. Plug in the USB to your PC
16. Go to [EspHome](https://web.esphome.io/) or another web flasher
17. Connect the board (you might need to hold the boot button and press the reset button)
18. Flash the firmware .bin file (if your web flasher requires an address use 0)
19. Install the lid
20. Follow the usual [First Time Setup](https://wiki.openshock.org/guides/openshock/first-setup)
21. **Enjoy** 😸

---

## Charging
- When the switch is turned off you can use it as a normal usb powered hub
- When you turn on the switch it becomes a portable hub
- You can charge it by turning on the switch and plugging in the USB
- The blue LED next to the USB port indicates charging
---

## Contact

Discord: Nova_Max

## Commercial Use
If you plan to use this design or any part of it for **commercial purposes**, please **contact me first**
