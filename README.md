# android-otg-wifi
register with termux-api your wifi-stick on your android



pkg update

pkg install root-repo

pkg install termux-api libusb clang

termux-usb -l

termux-usb -r [external device id]

nano usb.c

( copy and paste script from downloaded 'usb.c script' without bracket  )

gcc usb.c -lusb-1.0 -o usb

termux-usb -e ./usb [external device id/mac adress]

(sudo)ifconfig wlan1 up



                            .          .
                            .  TekHck  .
                            .          .
.
