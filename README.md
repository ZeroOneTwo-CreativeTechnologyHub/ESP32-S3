# ESP32-S3 Examples

A collection of example sketches for the **Seeed XIAO ESP32-S3** with the **Seeed Grove Breakout Board**. These examples cover Wi-Fi soft access points, servo control over a web interface, and device-to-device communication using ESP-NOW.

Built for beginners and anyone getting started with the XIAO ESP32-S3 platform.

---

## Hardware

| Component | Notes |
|---|---|
| [Seeed XIAO ESP32-S3](https://wiki.seeedstudio.com/xiao_esp32s3_getting_started/) | Compact ESP32-S3 board with Wi-Fi, BLE, and USB-C |
| [Seeed Grove Breakout Board](https://wiki.seeedstudio.com/Grove-Shield-for-Seeeduino-XIAO-Embedded-Battery-Management-Chip/) | Provides Grove connectors for easy sensor/actuator wiring |

Depending on the example, you may also need a servo motor, push button, LED, or other basic components.

---

## Examples

### ESP32_SoftAP

Sets up the XIAO ESP32-S3 as a **Wi-Fi Soft Access Point**. Connect to the ESP32's own Wi-Fi network directly from your phone or laptop — no router required. This is a good starting point for understanding how to create a local wireless interface.

**What you'll learn:** Creating a soft AP, setting an SSID and password, serving a basic web page.

---

### Servo_SoftAP

Builds on the soft access point example by adding **servo motor control via a web interface**. Connect to the ESP32's Wi-Fi, open a webpage in your browser, and control a servo remotely.

**What you'll learn:** Combining a soft AP web server with hardware control, reading HTTP requests, driving a servo with PWM.

**Extra hardware:** A servo motor connected via the Grove breakout or directly to a GPIO pin.

---

### Button_to_LED_ESPNOW

Uses **ESP-NOW** to send a button press from one ESP32 to another, wirelessly toggling an LED — with no Wi-Fi network needed. ESP-NOW is a fast, low-latency peer-to-peer protocol built into the ESP32.

**What you'll learn:** Pairing two ESP32 devices with ESP-NOW, sending and receiving data, reading a button input on one device and controlling an LED on another.

**Extra hardware:** Two XIAO ESP32-S3 boards (one with a button, one with an LED), or one board with both connected.

---

## Getting Started

1. **Install the Arduino IDE** (or your preferred editor with Arduino support).

2. **Add ESP32-S3 board support.** In the Arduino IDE, go to *File → Preferences* and add the following to *Additional Boards Manager URLs*:
   ```
   https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json
   ```
   Then go to *Tools → Board → Boards Manager*, search for **esp32** by Espressif Systems, and install it.

3. **Select your board.** Go to *Tools → Board* and choose **XIAO_ESP32S3**.

4. **Open an example.** Download or clone this repo, then open any of the `.ino` files in the Arduino IDE.

5. **Upload.** Connect your XIAO ESP32-S3 via USB-C and click Upload.

> **Tip:** If the board isn't recognised, you may need to hold the **BOOT** button while connecting USB, then release it once the port appears.

---

## Useful Links

- [XIAO ESP32-S3 Getting Started Guide](https://wiki.seeedstudio.com/xiao_esp32s3_getting_started/)
- [Grove Breakout Board Wiki](https://wiki.seeedstudio.com/Grove-Shield-for-Seeeduino-XIAO-Embedded-Battery-Management-Chip/)
- [ESP-NOW Documentation (Espressif)](https://docs.espressif.com/projects/esp-idf/en/stable/esp32s3/api-reference/network/esp_now.html)
- [Arduino-ESP32 GitHub](https://github.com/espressif/arduino-esp32)

---

## License

This project is licensed under the [MIT License](LICENSE). You're free to use, modify, and distribute these examples — just include the original copyright notice.

---

## Credits

Created by [ZeroOneTwo Creative Technology Hub](https://github.com/ZeroOneTwo-CreativeTechnologyHub).
