# Cudy P2 v2 OpenWrt patch

Custom OpenWrt patch for Cudy P2 v2 with MeiG SRM810-EU / SPRD PCIe modem support.

Tested baseline:

- OpenWrt 25.12.5

Patch file:

- `patches/cudy-p2-openwrt-25.12.5.patch`

This patch is based on work from:

- https://github.com/zekica/openwrt-sprd-pcie
- https://github.com/openwrt/openwrt/pull/23721

## Apply
```sh
git clone https://git.openwrt.org/openwrt/openwrt.git openwrt-p2-v2
cd openwrt-p2-v2
git checkout v25.12.5
git am /path/to/patches/cudy-p2-openwrt-25.12.5.patch
./scripts/feeds update -a
./scripts/feeds install -a
make defconfig
make -j$(nproc) V=s
