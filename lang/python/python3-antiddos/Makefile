# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python3-antiddos
PKG_VERSION:=v1.0
PKG_RELEASE:=1

PKG_SOURCE:=antiddos-v1.0.tar.gz
PKG_SOURCE_URL:=https://github.com/Hai-Phu/antiddos/releases/download/v1.0
PKG_HASH:=715481f321224e8b674ccc9d88b85b0264e7b36402bd2db30f24ab7dff612352

PKG_BUILD_DIR:=$(BUILD_DIR)/python3-antiddos-v1.0

PKG_MAINTAINER:=HaiPhu <haiphu@hcmut.edu.vn>
PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=LICENSE

HOST_PYTHON3_PACKAGE_BUILD_DEPENDS:=Cython

include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-antiddos
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:=Antiddos
  DEPENDS:=+python3-light
  VARIANT:=python3
endef

define Package/python3-antiddos/description
 AntiDDoS
endef

$(eval $(call Py3Package,python3-antiddos))
$(eval $(call BuildPackage,python3-antiddos))
