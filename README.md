# Android Device Tree for Samsung Galaxy Tab A8 10.5 (SM-X200)

LineageOS / AOSP device tree for Samsung Galaxy Tab A8 10.5 (2021) Wi-Fi (`gta8wifi` / `ums512_25c10`).

## Specifications
- **SoC:** Unisoc Tiger T618 (2x Cortex-A75 @ 2.0 GHz + 6x Cortex-A55 @ 2.0 GHz)
- **GPU:** Mali-G52 MP2 (Bifrost)
- **Display:** 1200 x 1920 (WUXGA) TFT, 240 DPI
- **Storage/RAM:** eMMC 5.1 / 3GB or 4GB LPDDR4x
- **Partitions:** System-as-root, Dynamic Partitions (6.84 GB Super)

## Kernel
Paired with [encipherdev/enciphered-kernel-4.14](https://github.com/encipherdev/enciphered-kernel-4.14).

## Build Setup
```bash
# Clone to device/samsung/gta8wifi
git clone https://github.com/encipherdev/android_device_samsung_gta8wifi device/samsung/gta8wifi
git clone https://github.com/encipherdev/android_vendor_samsung_gta8wifi vendor/samsung/gta8wifi
git clone https://github.com/encipherdev/enciphered-kernel-4.14 kernel/samsung/gta8wifi

. build/envsetup.sh
lunch lineage_gta8wifi-userdebug
mka bacon
```
