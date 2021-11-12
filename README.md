# hiltop_kernel_patches

The patches we apply when building a Linux kernel with the HILTOP.

All the extra hardware is in one big device tree overlay. We setup this to be used from the Pi's config.txt with dtoverlay=hiltop.

WARNING: Use a kernel that includes the commit 82a8ffba54d3 or you will hit a quiet out of bounds bug in the bcm2835 SPI controller's driver.
