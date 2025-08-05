# ICM-20948 Development Board

The **ICM-20948** is a low-power 9-axis MEMS motion tracking device that combines a 3-axis gyroscope, a 3-axis accelerometer, and a 3-axis magnetometer. This breakout board makes it easy to interface the ICM-20948 with your microcontroller via I²C or SPI, enabling a wide range of motion tracking applications like robotics, wearables, drones, and more.

## 📦 Features

* **9-axis sensor**:
  * 3-axis Accelerometer (±2/4/8/16 g)
  * 3-axis Gyroscope (±250/500/1000/2000 dps)
  * 3-axis Magnetometer (AK09916)
* **Ultra-low power consumption**
* **Digital Motion Processor (DMP)**
* **Communication Interfaces**:
  * I²C (up to 400 kHz)
  * SPI (up to 7 MHz)
* **Voltage Regulator**: Operates at 1.8–3.3V input
* **Onboard pull-up resistors for I²C**
* **Compact size**: Typically 1"x1"

## 📘 Documentation

* [ICM-20948 Datasheet (TDK InvenSense)](https://invensense.tdk.com/wp-content/uploads/2019/02/ds-000189-icm-20948-v1.3.pdf)
* [AK09916 Magnetometer Datasheet](https://www.akm.com/akm/en/file/datasheet/AK09916C.pdf)
* [Register Map and Programming Guide](https://invensense.tdk.com/wp-content/uploads/2020/04/RM-ICM-20948-v1.4.pdf)

## 🔌 Pinout

| Pin | Function                 |
| --- | ------------------------ |
| VIN | Power supply (1.8V–3.3V) |
| GND | Ground                   |
| SDA | I²C Data / SPI MOSI      |
| SCL | I²C Clock                |
| SDO | I²C Address / SPI MISO   |
| CS  | SPI Chip Select          |

## 🚀 Getting Started

### Requirements

* Microcontroller (Arduino, ESP32, Raspberry Pi, STM32, etc.)
* ICM-20948 Breakout Board
* Logic level compatibility (1.8V–3.3V)

### Libraries

* **Arduino**:

  * [SparkFun ICM-20948 Library](https://github.com/sparkfun/SparkFun_ICM-20948_ArduinoLibrary)
  * Install via Library Manager or clone via Git:

    ```bash
    git clone https://github.com/sparkfun/SparkFun_ICM-20948_ArduinoLibrary.git
    ```

* **Raspberry Pi (Python)**:

  * [RTIMULib2](https://github.com/richards-tech/RTIMULib2)
  * or write your own I²C interface using `smbus2`

## 🛠️ Applications

* Drone flight controllers
* Wearable fitness devices
* Gesture recognition
* Robotics
* VR/AR head tracking
* Automotive navigation systems

## ⚙️ Tips

* For best magnetometer performance, avoid placing the board near ferromagnetic materials or current-carrying wires.
* Use DMP features if you want to reduce processing load on your MCU (advanced).
* Calibration is key for accurate results (especially magnetometer).

## 📄 License

This project/documentation is released under the [MIT License](./LICENSE).

## 🤝 Contributing

Feel free to open issues, suggest improvements, or contribute code via pull requests.
