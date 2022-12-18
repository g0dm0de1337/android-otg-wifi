# android-otg-wifi
register with termux-api your wifi-stick on your android
#works on Termux !!



pkg update

pkg install root-repo

pkg install termux-api libusb clang

termux-usb -l

termux-usb -r [external device id/mac adress]

nano usbtest.c

( copy and paste script from downloaded folder,
'usb.c script' without bracket  )

gcc usbtest.c -lusb-1.0 -o usbtest

termux-usb -e ./usbtest [external device id/mac adress]

(sudo)ifconfig wlan1 up



                            .          .
                            .  TekHck  .
                            .          .
.
