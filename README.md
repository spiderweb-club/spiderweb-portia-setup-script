# spiderweb-portia Official Setup Script

This repository contains a Bash script for setting up prerequisites for the spiderweb-portia platform. The script is designed for various Linux distributions and handles necessary configurations, especially for systems with Nvidia GPUs.

## Getting Started

These instructions will guide you on how to use the setup script from this repository.

### Prerequisites

Ensure you have `curl` installed on your system to download the script.

- Run the following command to install if not installed already.<br>
  ```
  sudo apt install curl
  ```

### Installation

1. **Download the setup script**:

   ```bash
   curl -L https://github.com/spiderweb-club/spiderweb-portia-setup-script/raw/main/spiderweb-portia-setup.sh -o spiderweb-portia-setup.sh

   ```

2. Run the script:
   ```bash
   chmod +x spiderweb-portia-setup.sh && ./spiderweb-portia-setup.sh

   ```

## Script Overview

The `spiderweb-portia-setup.sh` script performs a series of operations:

- Sets global variables and detects the operating system and its version.
- Checks for Nvidia GPU presence and installs necessary drivers and CUDA toolkit based on the detected Linux distribution and version.
- Installs Docker and Docker Compose, along with setting up Nvidia Docker if an Nvidia GPU is detected.
- Adds the user to the Docker group.

## Supported Distributions

- Ubuntu (20.04, 22.04, 18.04)
- Debian (10, 11)

## Contributions

Contributions to this script are welcome. Please ensure that any pull requests or issues are relevant to the script's functionality and compatibility.

## Support

For support, please open an issue or contact our support team on [discord](https://discord.gg/kqFzFK7fg2)
