# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=numpy
PKG_VERSION:=1.20.1
PKG_RELEASE:=1

PKG_SOURCE:=numpy-1.20.1.zip
PKG_SOURCE_URL:=https://files.pythonhosted.org/packages/d2/48/f445be426ccd9b2fb64155ac6730c7212358882e589cd3717477d739d9ff
PKG_HASH:=3bc63486a870294683980d76ec1e3efc786295ae00128f9ea38e2c6e74d5a60a

PKG_BUILD_DIR:=$(BUILD_DIR)/numpy-$(PKG_VERSION)

PKG_MAINTAINER:=Philippe BIONDI <guillaume@valadon.net>
PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=LICENSE

HOST_PYTHON3_PACKAGE_BUILD_DEPENDS:=Cython

include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-numpy
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:=Scipy
  DEPENDS:=+python3-light
  VARIANT:=python3
endef

define Package/python3-numpy/description
  Composable command line interface toolkit
endef

$(eval $(call Py3Package,python3-numpy))
$(eval $(call BuildPackage,python3-numpy))
$(eval $(call BuildPackage,python3-numpy-src))
