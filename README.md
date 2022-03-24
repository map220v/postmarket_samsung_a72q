# postmarket_samsung_a72q
PostmarketOS for Samsung Galaxy A72

## Works
- USB Gadget mode
- Screen (simple-framebuffer)
- Hexagon 692 DSP (mpss)
- Wifi
- CPU (tlmm, clock controllers)
- UFS Storage
- SDHC (SDCard)
- IOMMU
- Some other things from sc7180.dtsi
## Broken
- GPU (Error: "A618: timeout waiting to drain ringbuffer 0 rptr/wptr = 0/C")
- Touchscreen (Error: "i2c txn timed out", "timeout abort_m_cmd")
