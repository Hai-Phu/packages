# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.

include $(TOPDIR)/rules.mk

PKG_NAME:=antiddos
PKG_VERSION:=v1.0
PKG_RELEASE:=1
PKG_LICENSE:=Apache-2.0

PKG_SOURCE:=$(PKG_NAME)-$(PKG_VERSION).tar.gz
PKG_SOURCE_URL:=https://github.com/Hai-Phu/antiddos/releases/download/$(PKG_VERSION)/$(PKG_SOURCE)
PKG_HASH:=715481f321224e8b674ccc9d88b85b0264e7b36402bd2db30f24ab7dff612352
PKG_BUILD_DIR:=$(BUILD_DIR)/$(PKG_NAME)-$(PKG_VERSION)

include $(INCLUDE_DIR)/package.mk

include ../python-package.mk
include ../python3-package.mk

# PKG_UNPACK:=$(HOST_TAR) -C $(PKG_BUILD_DIR) --strip-components=1 -xzf $(DL_DIR)/$(PKG_SOURCE)

define Package/python-vobject/Default
  SECTION:=net
  CATEGORY:=Network
  MAINTAINER:=Phu Nguyen-Phan-Hai <haiphu@hcmut.edu.vn>
  TITLE:=AntiDDoS
  URL:=https://github.com/Hai-Phu/antiddos/
  DEPENDS:=+python3-numpy +python3-scapy
endef

define Package/antiddos/description
 AntiDDoS
endef

define Build/Configure
endef

define Build/Compile
endef

$(eval $(call PyPackage,antiddos))
$(eval $(call BuildPackage,antiddos))
