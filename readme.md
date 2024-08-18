# Raspberry Pi Video Kiosk

This script turns Raspbian desktop system into a video kiosk. Tested on Raspbian 12 (bookworm) with LXDE desktop environment.

After setup and system reboot it will auto start VLC player and play video files from specified folder. Supports live playlist updates and hot ffmpeg video resizing.

Before first run update .env file with apropriate settings.

## Usage 

Setup video kiosk:

```shell
bash ./video-kiosk setup
sudo reboot now
```

This command will fix Raspbian to auto login, add autostart task and enable VNC server

Allowed commands

* setup - sets script up
* reset - clears script data and runs setup again
* stop - stops script
* start - starts script
* restart - restarts script
