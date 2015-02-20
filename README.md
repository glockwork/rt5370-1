rt5370
-------

RT5370 Wireless Lan Linux Driver AP enabled.


## Dependences for ArchLinux

```
sudo pacman -S linux-headers
```

Please read ***README_STA_usb*** about how to build it.


## insmod

```
sudo insmod os/linux/rt5370sta.ko
```

```
lsmod | grep rt
rt5370sta             793605  0 
rt2800usb              26171  0 
rt2x00usb              17642  1 rt2800usb
iTCO_vendor_support    12649  1 iTCO_wdt
rt2800lib              85279  1 rt2800usb
rt2x00lib              46262  3 rt2x00usb,rt2800lib,rt2800usb
mac80211              608652  4 rt2x00lib,rt2x00usb,rt2800lib,iwldvm
cfg80211              453926  4 iwlwifi,mac80211,rt2x00lib,iwldvm
crc_ccitt              12347  1 rt2800lib
parport_pc             26351  0 
parport                35749  2 ppdev,parport_pc
led_class              12855  3 rt2x00lib,hp_accel,iwldvm
usbcore               199382  8 btusb,uhci_hcd,uvcvideo,rt2x00usb,rt2800usb,ehci_hcd,ehci_pci,rt5370sta
```
