# postmarket_samsung_a72q
PostmarketOS for Samsung Galaxy A72

## Works
- USB Gadget mode
- Screen (simple-framebuffer)
- Hexagon 692 DSP (mpss)
- Wifi
- Bluetooth
- CPU (tlmm, clock controllers)
- UFS Storage
- SDHC (SDCard)
- IOMMU
- Battery (sm5714-fg)
- Some other things from sc7180.dtsi
## Broken
- GPU (Error: "A618: timeout waiting to drain ringbuffer 0 rptr/wptr = 0/C")
- Touchscreen (Error: "i2c txn timed out", "timeout abort_m_cmd")
- Panel/DPU (Errors: 
```
[drm:dpu_encoder_helper_register_irq:350] [dpu error]enc31 intf1 pp0 invalid IRQ index:-1
[drm:dpu_encoder_phys_cmd_control_vblank_irq [msm]] id:31 pp:0 enable=true/0
[drm:dpu_encoder_helper_register_irq:350] [dpu error]enc31 intf1 pp0 invalid IRQ index:-1
[drm:dpu_encoder_phys_cmd_control_vblank_irq [msm]] *ERROR* vblank irq err id:31 pp:0 ret:-22, enable true/0
...
[drm:dpu_encoder_frame_done_timeout:2088] [dpu error]enc31 frame done timeout
[drm:dpu_encoder_frame_done_timeout:2088] [dpu error]enc31 frame done timeout
[drm:dpu_encoder_frame_done_timeout:2088] [dpu error]enc31 frame done timeout
[drm:dpu_encoder_frame_done_timeout:2088] [dpu error]enc31 frame done timeout
[drm:dpu_encoder_frame_done_timeout:2088] [dpu error]enc31 frame done timeout
...
```
