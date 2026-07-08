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

From a clean OpenWrt 25.12.5 tree:

```sh
git am /path/to/patches/cudy-p2-openwrt-25.12.5.patch
