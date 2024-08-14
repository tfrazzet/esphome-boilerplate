# ESPHome Project Boilerplate

This repository contains a boilerplate for an ESPHome project. The main configuration file is `main.yaml`, which includes various components and settings for ESPHome devices.

## Table of Contents

- Overview
- Configuration Files
- Getting Started
- Components
- Contributing
- License

## Overview

This project is designed to provide a starting point for ESPHome configurations. It includes configurations for WiFi, sensors, logging, and various buses (I²C, SPI). The main configuration file is `main.yaml`, which imports all necessary components and settings.

## Configuration Files

### Main Configuration

- **File:** `main.yaml`
- **Description:** The main configuration file for the ESPHome project. It defines the device used and imports all necessary components and automations.

### WiFi Configuration

- **File:** `components/wifi.yaml`
- **Description:** Configures the WiFi settings for the ESPHome device. Remember to change the static IP address to avoid conflicts on the local network.

### Date Sensor Configuration

- **File:** `components/sensors/date.yaml`
- **Description:** Defines a text sensor for displaying the current date.

### Time Sensor Configuration

- **File:** `components/sensors/time.yaml`
- **Description:** Defines a text sensor for displaying the current time.

### Logger Configuration

- **File:** `components/logger.yaml`
- **Description:** Configures the logger component for ESPHome, used to log messages to the serial console.

### I²C Bus Configuration

- **File:** `components/buses/i2c.yaml`
- **Description:** Configures the I²C bus for ESPHome, used to communicate with various sensors and devices.

### SPI Bus Configuration

- **File:** `components/buses/spi.yaml`
- **Description:** Configures the SPI bus for ESPHome, used to communicate with various sensors and devices.

### Time Configuration

- **File:** `components/time.yaml`
- **Description:** Configures the time component for ESPHome, used to synchronize the time with an SNTP server.

## Getting Started

1. Clone the repository:
   ```   
   git clone https://github.com/tfrazzet/esphome-boilerplate.git YOUR-PROJECT_FOLDER
   cd YOUR-PROJECT_FOLDER
   ```   
2. Customize project data in **`common/config.yaml`**
2.1. Set node name
2.2. Giva a friendly name (for dashboard)
2.3. Set the location (for dashboard)

3. Include your device configuration in **`main.yaml`** packages section.

4. Rename **`secrets.yaml.template`** to **`secrets.yaml`** and insert your passwords.

5. Set wifi settings in substitutions inside **`components/wifi.yaml`**.

6. Customize the other components by changing the variables in the substituctions sections to suit your needs.

7. Connect your device and run 
   ```
   esphome run main.yaml
   ```

## Components
This boilerplate includes the following components:

* WiFi: Configures the WiFi settings for the ESPHome device.
* Date Sensor: Displays the current date.
* Time Sensor: Displays the current time.
* Logger: Logs messages to the serial console.
* I²C Bus: Communicates with various sensors and devices.
* SPI Bus: Communicates with various sensors and devices.
* Time: Synchronizes the time with an SNTP server.

**Where necessary each component has an initial substitutions section which can be used to customize its configuration.**

## Contributing
Contributions are welcome! Please fork this repository and submit a pull request with your changes.

## License
This project is licensed under the GPL v3 License. See the LICENSE file for details.

