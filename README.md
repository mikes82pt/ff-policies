# Firefox Policies Installation

This repository provides a `policies.json` file for configuring Firefox settings. You can use the instructions below to apply these policies to Firefox on both Windows and Linux.

## Prerequisites

- **Windows:** Administrator privileges required.
- **Linux:** `sudo` access required to install and modify files in system directories.

## Installation Instructions

### On Windows
1. Create the `distribution` folder if it doesn't exist:
    ```cmd
    if not exist "C:\Program Files\Mozilla Firefox\distribution" mkdir "C:\Program Files\Mozilla Firefox\distribution"
    ```

2. Download the `policies.json` file:
    ```cmd
    curl -s https://raw.githubusercontent.com/mikes82pt/ff-policies/refs/heads/main/policies.json -o "C:\Program Files\Mozilla Firefox\distribution\policies.json"
    ```

### On Linux

1. Create the `policies` directory if it doesn't exist:
    ```bash
    test -d "/etc/firefox/policies/" || sudo mkdir -p "/etc/firefox/policies/"
    ```

2. Download the `policies.json` file:
    ```bash
    sudo curl -s https://raw.githubusercontent.com/mikes82pt/ff-policies/refs/heads/main/policies.json -o /etc/firefox/policies/policies.json
    ```
