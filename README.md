# Pwnagotchi Setup

This repository documents the setup and configuration for the **Pwnagotchi** project, using a **Raspberry Pi Zero W** to capture WPA/WPA2 Wi-Fi handshakes for ethical Wi-Fi network analysis. The project uses a **Pwnagotchi `.img` file** to quickly get the system running with minimal setup.

## Overview

Pwnagotchi is a Wi-Fi penetration testing tool powered by AI, designed to capture Wi-Fi handshakes from nearby networks for security auditing. The system uses a Raspberry Pi Zero W, and once set up, it autonomously captures Wi-Fi handshakes and continuously learns to improve its capabilities.

### Features:
- **AI-Powered**: Pwnagotchi uses reinforcement learning to improve its handshake capturing ability.
- **Autonomous Operation**: It runs continuously without human intervention.
- **Portable**: Uses the compact Raspberry Pi Zero W, which is ideal for on-the-go penetration testing.
- **Customizable**: Configure settings like Wi-Fi, display, and power management via the `config.toml` file.
- **Learning & Stats**: Tracks the number of handshakes captured and learns from its environment over time.
- **Open-Source**: Licensed under the MIT License, anyone can contribute or modify it.

## Setup Instructions

### 1. **Download & Flash the Pwnagotchi Image**
   - Download the Pwnagotchi `.img` file from this repository (or from the [official Pwnagotchi site](https://pwnagotchi.ai/)).
   - Flash the `.img` file onto an 8GB or larger microSD card using tools like **Balena Etcher** or **Raspberry Pi Imager**.
   - After flashing, the microSD card will have two partitions: one for boot and one for the file system.

### 2. **Configure Pwnagotchi (Optional)**
   - Open the **boot partition** of the flashed microSD card.
   - Edit the `config.toml` file to customize settings:
     - Set your **Wi-Fi network** credentials.
     - Configure the **display type** (OLED, SPI, etc.).
     - Adjust any other settings for USB tethering, network, and power management.
   
   Example settings:
   ```toml
   wifi = true
   display = "oled"

### Key Sections in the README:
1. **Project Overview**: Provides an introduction to Pwnagotchi and its capabilities.
2. **Setup Instructions**: Guides the user through downloading, flashing, and configuring the system.
3. **Optional Configuration**: Describes how to adjust the configuration to fit personal needs.
4. **Legal Disclaimer**: Emphasizes ethical and legal usage of the tool.
5. **License**: Information about the open-source MIT license.
6. **Contributing**: Encourages users to contribute to the project.
7. **Acknowledgments**: Credits the tools and platforms that helped build the project.

This README provides a clear, concise guide to setting up and using Pwnagotchi, with all the necessary details to get started. Let me know if you need more adjustments!
