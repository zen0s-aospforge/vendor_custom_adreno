# Custom Adreno GPU Driver - Version 772

This repository contains a custom Adreno GPU driver package for Android devices, specifically version 772. It includes proprietary blobs and configurations for enhanced GPU performance and Vulkan support.

## Features
- Vulkan 1.3 support via `android.hardware.vulkan.version-1_3.xml`
- Firmware files for Adreno 650 (a650_gmu.bin, a650_sqe.fw)
- Kernel-based compute (KBC) binaries
- EGL and OpenGL ES libraries for both 32-bit and 64-bit architectures
- Hardware abstraction layer (HAL) for Vulkan
- Additional utilities and profiles for Adreno GPUs

## Installation
To include this driver in your Android build, add the following hook line to your device's `device.mk` 
```markdown
$(call inherit-product, vendor/custom/adreno/gpu-vendor.mk)
```
