linux-kirkwood-3.8
==================

Kernel 3.8 for Marvell Kirkwood devices

NOTE: I have abandoned this PKGBUILD.
This PKGBUILD was based on kernel 3.8-rc2, there were many changes meanwhile and I don't plan on spending more time to adjust these patches.
The reason is that I don't see any reason for patching the kernel the hard way instead of switching to device trees.
Kernel patching will eventually become harder with 3.9 which will probably add a cool new feature: cpufreq-driver to switch clocks for Kirkwood devices (CPU-clock and DDR-clock)
This feature will be device-tree-only I guess, so it would be the best option to abandon heavy kernel patching.

Based on Arch Linux ARM kernel 3.6.
See https://github.com/archlinuxarm/PKGBUILDs/tree/master/core/linux-kirkwood

This builds as linux-kirkwood and linux-headers-kirkwood.

Kernels > 3.1 require a newer bootloader than some Kirkwood devices originally came with.

This kernel builds for every kirkwood platform Arch Linux ARM kernel supports. However,
I did only test it on a GoFlex Net, don't blame me if your device becomes unbootable or explodes etc. pp.
