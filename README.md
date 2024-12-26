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
