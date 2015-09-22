#Download Lastest GCC in http://downloads.openwrt.org/snapshots/trunk/
#This is a demo for Netgear WNDR3800(AR71XX)

#TODO : Change the location for your GCC's location
CC=~/OpenWrt-SDK-15.05-ar71xx-generic_gcc-4.8-linaro_uClibc-0.9.33.2.Linux-x86_64/staging_dir/toolchain-mips_34kc_gcc-4.8-linaro_uClibc-0.9.33.2/bin/mips-openwrt-linux-gcc
CFLAGS=-Os -Wall
INCLUDE=~/OpenWrt-SDK-15.05-ar71xx-generic_gcc-4.8-linaro_uClibc-0.9.33.2.Linux-x86_64/staging_dir/toolchain-mips_34kc_gcc-4.8-linaro_uClibc-0.9.33.2/include

all:sxplugin.so hainan_sxplugin.so

sxplugin.so:
	$(CC) $(CFLAGS) sxplugin.c -fPIC -I$(INCLUDE) -shared -o sxplugin.so

hainan_sxplugin.so:
	$(CC) $(CFLAGS) hainan_sxplugin.c -fPIC -I$(INCLUDE) -shared -o hainan_sxplugin.so
