# postmarket_samsung_a72q
PostmarketOS for Samsung Galaxy A72

## Works
- USB Gadget mode
- Display (samsung,s6e3fc3-ams667ym01)
- Modem (works only with modemmanager. ofone doesn't seem to work)
- Wifi
- Bluetooth
- CPU (tlmm, clock controllers)
- UFS Storage
- SDHC (SDCard)
- IOMMU
- Battery (sm5714-fg)
- Touchscreen
- Some other things from sc7180.dtsi
## Broken
- GPU (Error: "A618: timeout waiting to drain ringbuffer 0 rptr/wptr = 0/C")
- Display Brightness
- Display Sleeep (after sleep display won't start. Workaround: reboot phone
Error: "*ERROR* encoder is disabled id=31, intr=3, irq=41")
## Bugs
- Modem sometimes can't start at boot.
