# SPDX-License-Identifier: GPL-2.0-only
#
# Copyright (C) 2006-2007 OpenWrt.org

include $(TOPDIR)/rules.mk
include $(INCLUDE_DIR)/target.mk
include $(INCLUDE_DIR)/default-packages.mk

export TARGET_BUILD=1

prereq clean download prepare compile install oldconfig menuconfig nconfig xconfig update refresh dtb: FORCE
	@+$(NO_TRACE_MAKE) -C $(firstword $(wildcard feeds/$(BOARD) $(BOARD))) $@
