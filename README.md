# Arduino on ESP-IDF Example for ESP32-C6

This project demonstrates how to run Arduino as part of an ESP-IDF project for the ESP32-C6. By integrating Arduino into ESP-IDF, you can combine the simplicity of Arduino with the advanced functionality of ESP-IDF, offering greater flexibility for your projects.

This project is an example of how to use Arduino running in ESP-IDF. If you would like an overview of the different options on the ESP32-C6 I have an overview of my different example reposoties on (a GitHub Gist that can be found on this link.)[https://gist.github.com/Graunephar/57a9882cb3a2ab98be8d63a59ab16ef3]

## What This Repository Contains

This repository provides an example of using Arduino in an ESP-IDF project, specifically running a simple **blink program**. It demonstrates how to:
- Use Arduino's `setup()` and `loop()` functions within the ESP-IDF environment.
- Leverage ESP-IDF features, like advanced configurations and hardware control.

Simply clone it down, and run it on your ESP32-C6 and you should be good to go.

## Two Ways to Run Arduino on ESP32-C6

Arduino can be used in two distinct ways on the ESP32-C6, which is essential to understand for choosing the right approach for your needs.

### 1. **Pure Arduino Framework**
In this approach, Arduino is used as the sole framework. It’s typically run using the Arduino IDE or PlatformIO in Arduino-only mode. This is the standard way of running Arduino and focuses exclusively on its libraries and APIs. If you would rather do this I have an example of how to do it (in the repo here)[https://github.com/Graunephar/Esp32-C6-blink-in-pure-Arduino-framework-with-PlatformIO]

- **Use Case**: Ideal for simpler applications or when you don’t need advanced control over the ESP32-C6 hardware.
- **Features**: Limited to Arduino's functionality without access to ESP-IDF-specific features like ULP or FreeRTOS configurations.

### 2. **Arduino as a Component in ESP-IDF**
This project demonstrates the second approach, where Arduino is integrated as a component in an ESP-IDF project. In this setup:
- ESP-IDF handles the build process, and Arduino’s functions (`setup()` and `loop()`) are incorporated into the broader ESP-IDF environment.
- You gain access to both Arduino APIs and advanced ESP-IDF features, such as ultra-low-power operations, precise hardware configurations, and custom peripheral management.

- **Use Case**: Suitable for advanced applications requiring both Arduino’s simplicity and ESP-IDF’s advanced hardware features.