# Mr. Robot Micropad

**Mr. Robot Micropad** is a quirky, minimalist two-key input device designed for Home Assistant users.

Built around a Wemos D1 Mini (ESP8266) and a 0.96" OLED display, this little guy blinks, glances, and looks around the room with expressive animated eyes. Each key can trigger up to eight unique Home Assistant actions using single, double, triple tap, or long-press. Mount it anywhere with magnets, and customize it with your own keycaps, colors, and plate materials — even the exposed wiring becomes part of the aesthetic.

---

## 📸 Project Photo

![Mr. Robot Micropad Photo](images/micropad.jpg)

---

## 🎞️ Eye Animation Preview

![OLED Eye Animation](images/eye_animation.gif)

---

## Features

* **Two customizable keys** (single, double, triple tap + long-press)
* **Animated OLED display** with expressive idle behavior
* **Magnetic mounting**
* **Full Home Assistant integration** via ESPHome
* **Highly customizable aesthetic** through components and wiring

---

## Bill of Materials (BOM)

| Component                                 | Quantity              |
| ----------------------------------------- | --------------------- |
| ESP32 (ESP8266) Wemos D1 Mini             | 1                     |
| 0.96-inch I²C OLED Display (SSD1306/1315) | 1                     |
| MX Mechanical Switches                    | 2                     |
| MX-Compatible Keycaps                     | 2                     |
| 28 AWG Wire                               | As needed             |
| M1.6 × 4mm Button Head Screws             | 6                     |
| M1.6 × 3mm Heat Set Inserts               | 6                     |
| 8 × 1.6mm Magnets                         | 4 *(or 8 with mount)* |

*Note: You can use any I²C OLED based on the SSD1306 or SH1106 controller. Either driver is supported with minimal config changes.*

---

## Wiring Diagram

| Component    | Wire Color | ESP8266 Pin |
| ------------ | ---------- | ----------- |
| Switch A +   | Yellow     | D5 (GPIO14) |
| Switch A GND | Black      | GND         |
| Switch B +   | Yellow     | D6 (GPIO12) |
| Switch B GND | Black      | GND         |
| OLED VCC     | Red        | 3V3         |
| OLED GND     | Black      | GND         |
| OLED SDA     | Blue       | D2 (GPIO4)  |
| OLED SCL     | White      | D1 (GPIO5)  |

---

## Assembly & Setup

1. **Print all components**
   Download STL files from Printables:
   👉 [Mr. Robot Micropad on Printables](https://www.printables.com/model/1329568-mr-robot-micropad-a-two-button-smart-assistant-wit)

2. **Install magnets and heat-set inserts**
   Press-fit magnets into their designated slots. Install M1.6 heat-set inserts using a soldering iron.

3. **Mount the MX switches**
   Snap your mechanical switches into the printed switch plate.

4. **Wire the components**
   Use 28 AWG wire and follow the wiring diagram above to connect the switches and OLED display to the ESP8266.

5. **Assemble the enclosure**
   Mount the ESP8266 first, followed by the switch plate and OLED display. Use M1.6×4mm screws to secure components.

6. **Connect to your computer**
   Plug in the ESP8266 using the USB-C port.

7. **Flash the firmware**
   Use [ESPHome](https://esphome.io) to flash the firmware. A sample YAML config is included in this repo to get you started.

---

## License

This project is licensed under the [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-sa/4.0/).

---

Let me know if you’d like help embedding actual media or auto-generating a preview thumbnail for GitHub display.
