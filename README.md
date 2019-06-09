# WiFi support for the [OrangePi RK3399](http://www.orangepi.org/Orange%20Pi%20RK3399/)

Assuming Ubuntu 16.04 build from www.orangepi.org

1. Copy `fw_bcm4356a2_ag.bin` to `/system/etc/firmware`
1. Copy `nvram_ap6356.txt` to `/system/etc/firmware`
1. Mount `/dev/mmcblk1p6` to `/boot`
1. Back up `/boot/rk3399-orangepi.dtb` and `Image`
1. Copy `rk3399-orangepi.dtb` from this repo into `/boot`
1. Copy `Image` from this repo into `/boot`
1. Reboot
1. You should see a `wlan0` interface from `ip link`
