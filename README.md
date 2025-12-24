# ESP8266 OLED Slot Machine

A retro-style 3-reel slot machine game built for the **ESP8266** (NodeMCU/Wemos D1 Mini) using an **SSD1306 OLED** display. 

## Features
* **Save System:** High scores and win history are saved to EEPROM.
* **Double or Nothing:** Gamble your winnings after a successful spin.
* **Animations:** Smooth reel spinning, win flashes, and a "Jackpot" sequence.
* **Sound & Light:** Integrated buzzer tones and LED feedback.

## Hardware Components
* **Microcontroller:** ESP8266 (e.g., NodeMCU)
* **Display:** 128x64 I2C SSD1306 OLED
* **Buttons:** 2x Tactile buttons (Spin/Collect & History/Gamble)
* **Feedback:** 3x LEDs and 1x Passive Buzzer

## Pin Mapping
| Component | Pin | Function |
|-----------|-----|----------|
| OLED SDA  | D5  | I2C Data |
| OLED SCL  | D6  | I2C Clock|
| Button 1  | D3  | Spin / Collect / Reset |
| Button 2  | D1  | History / Gamble |
| Buzzer    | D2  | Audio Feedback |

## Libraries Required
To compile this project, you will need the following libraries in your Arduino IDE:
1. `Adafruit_GFX`
2. `Adafruit_SSD1306`
3. `Wire` (Built-in)
4. `EEPROM` (Built-in)
