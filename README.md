# Pwnagotchi Setup for Raspberry Pi 4 & Raspberry Pi Zero W

This repository provides a step-by-step guide to set up **Pwnagotchi** on a **Raspberry Pi 4** or **Raspberry Pi Zero W**. Pwnagotchi is an AI-powered Wi-Fi penetration testing tool that captures WPA/WPA2 Wi-Fi handshakes.

## Requirements

Before setting up Pwnagotchi, make sure you have the following:
- **Raspberry Pi 4** or **Raspberry Pi Zero W** (or any other supported Raspberry Pi model)
- **microSD card** (at least 8GB recommended)
- **Wi-Fi adapter** (if using Raspberry Pi Zero W)
- **micro-USB power supply** (5V 2A for Pi Zero W and Pi 4)
- **OLED display** or other supported display
- **Keyboard and Monitor** (optional for initial setup via SSH)

## Step 1: Download the Pwnagotchi Image

1. Go to the official Pwnagotchi website: [Pwnagotchi](https://pwnagotchi.ai/) to download the latest `.img` file for Raspberry Pi.
2. Alternatively, you can download the `.img` file from this repository.

## Step 2: Flash the Image to the microSD Card

You will need to flash the `.img` file onto your microSD card. Here’s how you can do it using **Balena Etcher** or **Raspberry Pi Imager**.

### Using **Balena Etcher**:
1. Download **Balena Etcher** from [here](https://www.balena.io/etcher/).
2. Insert your **microSD card** into your computer.
3. Open **Balena Etcher** and select the downloaded **Pwnagotchi `.img` file**.
4. Select your **microSD card** as the target.
5. Click **Flash** to begin the flashing process.
6. Once complete, safely eject the microSD card from your computer.

### Using **Raspberry Pi Imager**:
1. Download **Raspberry Pi Imager** from [here](https://www.raspberrypi.org/software/).
2. Open **Raspberry Pi Imager**, select **Use custom** and choose the **Pwnagotchi `.img` file**.
3. Select the **microSD card** and click **Write** to flash the image.

## Step 3: Configure Pwnagotchi (Optional)

Once the image is flashed onto the microSD card, you can configure some settings before booting.

1. Insert the **microSD card** into your computer and navigate to the **boot partition**.
2. Open the **config.toml** file in a text editor.
3. Configure settings like Wi-Fi, display type, and other preferences:
   - Set your **Wi-Fi network** credentials.
   - Select your display type (`oled`, `spi`, etc.).
   - Set other configurations like enabling USB tethering or power management.

   Example settings:
   ```toml
   wifi = true
   display = "oled"
