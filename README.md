# Digital Shop Multitool

A custom-built, 3D-printed handheld multifunction shop tool powered by an ESP32-C3 SuperMini, featuring dual OLED displays and a shared I²C sensor bus integrating laser distance measurement, non-contact infrared temperature sensing, color analysis, and a gyroscope-based digital level.

## Hardware & Components
* **Microcontroller:** ESP32-C3 SuperMini (USB-C)
* **Displays:** 
  * 0.91-inch SSD1306 OLED (128×32, I²C `0x3C`)
  * 0.96-inch SSD1306 OLED (128×64, I²C `0x3D`)
* **Sensors (Shared I²C Bus on GPIO 10 SDA / GPIO 9 SCL):**
  * **VL53L1X:** Time-of-Flight (ToF) laser distance sensor (`0x29`)
  * **MPU-6050:** 6-axis accelerometer & gyroscope (`0x68`)
  * **MLX90614:** Non-contact infrared thermometer (`0x5A`)
  * **TCS34725:** RGB color sensor (`0x29`)
* **Enclosure:** Custom 3D-printed handheld housing
