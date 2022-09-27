# Video Capture with Loop Card on Ubuntu 16.04
###### tags: `Ubuntu` `Video Capture` `Ubuntu 16.04`


1. UVC driver installation (Official website: https://www.ideasonboard.org/uvc/)

    * Clone Linux driver from https://git.linuxtv.org/media_build.git
        ```
        git clone git://linuxtv.org/media_build.git
        ```
    * Build driver images
        ```
        cd media_build/

        ./build
        ```
    * Install driver
        ```
        sudo make install
        ```
    * Restart Ubuntu
    * Plug video capture card to USB port
    * Check if the device is activated
        ```
        # lsusb
        ```
        or
        ```
        # ls /dev/video*
        ```

2. OBS application installation (Official website: https://obsproject.com/)
    * Check the install instructions of OBS WiKi
        https://obsproject.com/wiki/install-instructions#linux

    Refer from above link:
    >NOTE: OpenGL 3.3 or later is required to use OBS Studio on Linux.
    You can check what version of OpenGL is supported by your system by typing:
    **glxinfo | grep "OpenGL"** on Terminal.
    >
    >Please note that OBS Studio does not work on Chrome OS.
    >
    >xserver-xorg version 1.18.4 or newer is recommended to avoid potential performance issues with certain features in OBS, such as the fullscreen projector.
    >
    >FFmpeg is required. If you do not have the FFmpeg installed (if you're not sure, then you probably don't have it), you can get it with the following commands:
    >
    >```
    >sudo apt install ffmpeg
    >```
    >If you want virtual camera support you need v4l2loopback-dkms installed. You can install it with the following command :
    >
    >```
    >sudo apt install v4l2loopback-dkms
    >```
    >
    >Make sure you enabled the multiverse repo in Ubuntu's software center (NOTE: On newer versions of Ubuntu, adding a repository automatically apt updates.) Then you can install OBS with the following commands:
    >
    > ```
    > sudo add-apt-repository ppa:obsproject/obs-studio
    > sudo apt update
    > sudo apt install obs-studio
    > ```

