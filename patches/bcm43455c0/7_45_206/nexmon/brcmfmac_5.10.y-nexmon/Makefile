#
# Makefile fragment for Broadcom 802.11n Networking Device Driver
#
# Copyright (c) 2010 Broadcom Corporation
#
# Permission to use, copy, modify, and/or distribute this software for any
# purpose with or without fee is hereby granted, provided that the above
# copyright notice and this permission notice appear in all copies.
#
# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
# WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
# MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY
# SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
# WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION
# OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN
# CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.

ccflags-y += \
	-I$(NEXMON_ROOT)/patches/bcm43455c0/7_45_206/nexmon/brcmfmac_5.10.y-nexmon	\
	-I$(NEXMON_ROOT)/patches/bcm43455c0/7_45_206/nexmon/brcmfmac_5.10.y-nexmon/include \
	-DDEBUG

obj-$(CONFIG_BRCMFMAC) += brcmfmac.o
brcmfmac-objs += \
		cfg80211.o \
		chip.o \
		fwil.o \
		fweh.o \
		p2p.o \
		proto.o \
		common.o \
		core.o \
		firmware.o \
		feature.o \
		btcoex.o \
		vendor.o \
		pno.o \
		debug.o
brcmfmac-$(CONFIG_BRCMFMAC_PROTO_BCDC) += \
		bcdc.o \
		fwsignal.o
brcmfmac-$(CONFIG_BRCMFMAC_PROTO_MSGBUF) += \
		commonring.o \
		flowring.o \
		msgbuf.o
brcmfmac-$(CONFIG_BRCMFMAC_SDIO) += \
		sdio.o \
		bcmsdh.o
brcmfmac-$(CONFIG_BRCMFMAC_USB) += \
		usb.o
brcmfmac-$(CONFIG_BRCMFMAC_PCIE) += \
		pcie.o
brcmfmac-$(CONFIG_BRCM_TRACING) += \
		tracepoint.o
brcmfmac-$(CONFIG_OF) += \
		of.o
