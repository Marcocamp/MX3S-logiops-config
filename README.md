[English](README.md) | [Italiano](README.it.md)
# 🖱️ Logiops Config for MX Master 3S


[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/Marcocamp/MX3S-logiops-config?style=social)](https://github.com/Marcocamp/MX3S-logiops-config/stargazers)




**Description:** This repository offers a [logiops](https://github.com/PixlOne/logiops) configuration that implements the use of Logitech MX Master 3S gestures.

## Features
Profile tested for Ubuntu 22.04
- **Side scroll wheel:** Volume control
- **Gesture button:** Show desktop
- **Gesture button + up:** Open default terminal
- **Gesture button + left:** Switch to left desktop
- **Gesture button + right:** Switch to right desktop

## Installation Instructions
Follow these simple steps to start the configuration:


1. **Install logiops:** follow the instructions from the [official repository](https://github.com/PixlOne/logiops) to install the package
2. **Clone Repository:** Open your terminal and run:
    ```bash
    git clone https://github.com/Marcocamp/MX3S-logiops-config.git
    ```
3. **Applying Configuration File:** This step requires root permissions (`sudo`).

    **Backup:** Run this command to save the current configuration:
    ```bash
    sudo cp /etc/logid.cfg /etc/logid.cfg.bkp 
    ```
    **Copy New File:** Copy the `logid.cfg` file found in the cloned directory to the system path:
    ```bash
    sudo cp logid.cfg /etc/logid.cfg 
    ```
    **Restart and Verify Service:** Reload the services to apply changes in real time:
    ```bash
    sudo systemctl restart logid 
    sudo systemctl status logid
    ```
4. **Test Configuration:** Try using the gesture button or changing the volume



## Contribution and Support
Found a bug or have improvements to suggest? Feel free to:
1. Create a `Branch` for your changes.
2. Add a *Pull Request* (PR) directly to this repository.


**Contacts:**
If you need assistance or want to see my other projects, visit my GitHub profile: 
 [Marcocamp](https://github.com/Marcocamp) 


Thanks for visiting my repository! I hope this configuration is useful to you.
