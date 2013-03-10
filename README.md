DhollmenCM_kernel
=================

Samsung Galaxy Tab 2 Kernel version 3.0.31

Compatible Cyanogenmod 10.1 - 4.2.2 


1. How to Build:
   

  - get Toolchain
      From Codesourcery site( http://www.codesourcery.com )
      recommand : 2010q1 version.
  - edit Makefile
      edit  "CROSS_COMPILE" to right toolchain path(You downloaded).
             example:  CROSS_COMPILE ?= /opt/toolchains/arm-2010q1/bin/arm-none-linux-gnueabi-
  - make
      cd kernel_src
      make ARCH=arm {defconfig_file}
      make ARCH=arm
 
   
   defconfig_files
   
      - dhollmen_P51XX_defconfig     : Normal Tab2 10.1 inch
      - dhollmen_P31XX_defconfig     : Normal Tab2  7   inch
      
      - dhollmen_P51XXHOT_defconfig  : Overcloked Tab2 10.1 inch
      - dhollmen_P31XXHOT_defconfig  : Overcloked Tab2  7   inch


2. Output files
   ------------
   - kernel  : arch/arm/boot/zImage
   - modules : drivers/*/*.ko
