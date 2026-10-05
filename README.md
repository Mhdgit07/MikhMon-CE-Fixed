# MikhMon CE Fixed

MikhMon CE Fixed is a Windows-ready distribution of MikhMon CE with selected fixes and improvements for a smoother local installation and operation.

This repository provides a self-contained Windows package including the MikhMon application, PHP runtime, and the MikhMon CE server launcher.

## Features

- Windows-ready distribution
- Bundled PHP runtime — no separate PHP installation required
- MikhMon CE included
- Fixed daily and monthly selling reports
- Fixed dashboard sales calculations for Today and This Month
- Fixed Traffic Monitor tooltip displaying invalid NaN values
- Clean default configuration
- No personal router configuration included
- No personal MikroTik credentials included

## Included

MikhMonCE-Windows/
- MikhMonCE_Server.exe
- php/
- mikhmon-ce/

## Installation

1. Download or clone this repository.
2. Open the MikhMonCE-Windows folder.
3. Run MikhMonCE_Server.exe.
4. Open the local MikhMon CE interface in your browser.

Default MikhMon credentials:

Username: admin
Password: admin

Important: Change your credentials and configure your MikroTik router before using MikhMon in production.

## Router Configuration

After launching MikhMon:

1. Log in with the default MikhMon credentials.
2. Open the router configuration section.
3. Add your own MikroTik router.
4. Enter your router IP address, API port, username and password.
5. Test the connection.
6. Configure your hotspot, users, profiles and other settings.

No personal router configuration from the developer is included in this distribution.

## Fixes Included

### Selling Report

The daily and monthly selling reports were corrected to reliably retrieve and filter MikhMon sales scripts by date.

### Dashboard

The dashboard sales indicators for Today and This Month were corrected to use reliable date-based sales data.

### Traffic Monitor

The traffic monitor tooltip was corrected to prevent invalid values such as:

NaN undefined

when traffic values are zero.

## Requirements

- Windows 10 or later
- Network access to your MikroTik router
- A MikroTik router configured for API access

No separate PHP installation is required because PHP is included in the distribution.

## Security

Do not publish or share:

- MikroTik administrator passwords
- MikhMon router credentials
- API credentials
- Private network configuration
- Production configuration files
- Session files or logs containing sensitive information

This repository intentionally contains a clean default configuration.

## Repository Structure

MikhMon-CE-Fixed/
- .gitignore
- MikhMonCE-Windows/
  - MikhMonCE_Server.exe
  - php/
  - mikhmon-ce/
- README.md
- LICENSE

## Project Status

This is a community-maintained fixed distribution intended to make MikhMon CE easier to deploy on Windows and to provide corrections for specific issues encountered in the original distribution.

The original MikhMon CE project and its respective authors retain their original rights and credits.

## Disclaimer

Use this software at your own risk.

Always make a backup of your MikhMon and MikroTik configuration before making significant changes.

The fixes included in this repository are provided in good faith and should be tested in your own environment before being used in production.

## Credits

This project is based on MikhMon CE.

Full credit for the original MikhMon project goes to its original authors and contributors.

This repository is not intended to replace or claim ownership of the original MikhMon project.

---

MikhMon CE Fixed — Windows distribution
