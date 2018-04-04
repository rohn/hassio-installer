# Hass.io on Raspberry Pi 3 B+

This script will install all [requirements], and then install [Hass.io]. Please report any [issues] that experience.

## Requirements

* [Raspberry Pi 3 B+]
* [Raspbian Stretch Lite]

## Instructions

1. Flash the latest [Raspbian Stretch Lite] image.
2. Run this as root user (`sudo su`):

```bash
curl -sL https://raw.githubusercontent.com/dale3h/hassio-installer/master/hassio_rpi3bp | bash -s
```

## Useful Tips

- Be sure to secure your Raspberry Pi by disabling SSH and changing the password for `pi` user.
- If you plan to install via SSH, be sure to create a file named `ssh` on your SD card in `/boot` to enable SSH on first boot.
- If you plan to connect via WiFi, be sure to setup your `wpa_supplicant.conf` file in `/boot` prior to your first boot.

## Known Issues

- **Bluetooth BCM43xx** add-on does not work
- **SSH server** add-on (from **Official add-ons**) does not work

[Hass.io]: https://www.home-assistant.io/hassio/
[issues]: /issues
[Raspberry Pi 3 B+]: http://a.co/ciXqByX
[Raspbian Stretch Lite]: https://downloads.raspberrypi.org/raspbian_lite_latest
[requirements]: https://github.com/home-assistant/hassio-build/blob/master/install/README.md#requirements
