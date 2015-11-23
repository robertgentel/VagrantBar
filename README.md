# Vagrant Bar

## Overview

Vagrant Bar is a simple wrapper to the Vagrant command line tool to manage machines registered with Vagrant - supporting ALL providers

![Screenshot](https://raw.githubusercontent.com/BipSync/VagrantBar/master/Screenshot.png)

## Requirements

* OS X 10.9
* Vagrant 1.6+ (any providers)
 * http://www.vagrantup.com

## Download

https://github.com/BipSync/VagrantBar/releases/download/1.20/Vagrant.Bar.zip


Version History|Notes
----|----
1.20 | Fixed vagrant location detection, thanks malthejorgensen!
1.19 | Add ability to display path instead of ID of running machines. Correctly detect OSX Dark Mode at startup and on change. Fixed global status parsing
1.18 | Click machine name to SSH
1.17 | Yosemite Black Status Bar support
1.16 | Further performance improvements
1.15 | Performance improvements after hours of use
1.14 | No longer shows '0' next to the icon
1.13 | Fix for issue https://github.com/BipSync/VagrantBar/issues/6
1.12 | Improvements from YungSang!
1.11 | Fix bug with out-of-date machine statuses
1.10 | Now displays the list of machines without any delay by parsing the machine index directly, falls back to old method, handles no machines correctly, faster status refresh rate
1.8 | Now shows the number of running machines (can be disabled, see below)
1.7 | Fixed incorrect statuses & path, fixed a bug with paths with spaces in the name
1.6 | Updated icons, fixed incorrect menu position
1.5 | Added retina icons, fixed missing image when asking for passwords
1.4 | Configurable icon, SSH application, check for updates. Updated icons. Now check for updates a maximum of once an hour
1.3 | Update notification
1.2 | Connect to a machine via SSH
1.1 | Vagrant Bar now verifies the Vagrant version on startup
1.0 | First release

## Installation
1. Copy "Vagrant Bar.app" to /Applications
2. Run from there
3. Optionally drag into "Login Items" under "System Preferences"/"Users & Groups" to autostart on login

## Configuration

Open a Terminal and run the following commands, then restart Vagrant Bar

Value|Command
---|---
Mono status bar icon|`defaults write bipsync.Vagrant-Bar monoIcon -bool true`
Use a different Terminal|`defaults write bipsync.Vagrant-Bar terminalAppName -string TERMINALAPPNAME`
Disable update checking|`defaults write bipsync.Vagrant-Bar checkForUpdates -bool false`
Disable displaying number of running machines|`defaults write bipsync.Vagrant-Bar displayRunningMachines -bool false`
Display path of running machines instead of ID|`defaults write bipsync.Vagrant-Bar displayPath -bool true`
