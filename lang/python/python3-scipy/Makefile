# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=scipy
PKG_VERSION:=1.7.3
PKG_RELEASE:=1

PKG_SOURCE:=scipy-1.7.3.tar.gz
PKG_SOURCE_URL:=https://files.pythonhosted.org/packages/61/67/1a654b96309c991762ee9bc39c363fc618076b155fe52d295211cf2536c7
PKG_HASH:=ab5875facfdef77e0a47d5fd39ea178b58e60e454a4c85aa1e52fcb80db7babf

PKG_BUILD_DIR:=$(BUILD_DIR)/Scipy-$(PKG_VERSION)

PKG_MAINTAINER:=Daniel Golle <daniel@makrotopia.org>
PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=LICENSE

include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-scipy
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:=Scipy
  DEPENDS:=+python3-light
  VARIANT:=python3
endef

define Package/python3-scipy/description
  Composable command line interface toolkit
endef

$(eval $(call Py3Package,python3-scipy))
$(eval $(call BuildPackage,python3-scipy))
$(eval $(call BuildPackage,python3-scipy-src))
