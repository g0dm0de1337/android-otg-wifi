# android-otg-wifi
register with termux-api your wifi-stick on your android



pkg update

pkg install root-repo

pkg install termux-api libusb clang

termux-usb -l

termux-usb -r [external device id]

nano usbtest.c

( copy and paste script from downloaded 'usb script' without bracket  )

gcc usbtest.c -lusb-1.0 -o usbtest

termux-usb -e ./usbtest [external device id]

sudo ifconfig wlan1 up



                            .          .
                            .  TekHck  .
                            .          .
.
