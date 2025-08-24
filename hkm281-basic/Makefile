# Copyright (c) 2023 LENAR

include $(TOPDIR)/rules.mk

PKG_NAME:=hkm281-basic
PKG_VERSION:=1.0
PKG_RELEASE:=1

PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=LENAR <https://phcorner.org/members/1875125/>
PKG_ARCH:=mipsel_24kc

include $(INCLUDE_DIR)/package.mk

define Package/$(PKG_NAME)
	SECTION:=custom
	CATEGORY:=Packages
	TITLE:=HKM281 Basic
	URL:=https://github.com/0x4C334E3438/My_PKG
endef

define Package/$(PKG_NAME)/description
	Configuration and scripts for ORBITPRO HKM281 OpenWrt router.
endef

define Build/Compile
	# This is a binary package, nothing to compile
endef

define Package/$(PKG_NAME)/install
	$(CP) -a ./files/* $(1)/
endef

$(eval $(call BuildPackage,$(PKG_NAME)))
