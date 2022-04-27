# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=protobuf
PKG_VERSION:=3.20.0
PKG_RELEASE:=1

PKG_SOURCE:=protobuf-3.20.0.tar.gz
PKG_SOURCE_URL:=https://files.pythonhosted.org/packages/6d/3e/40c56d21154a1f3ababb69f675333d7fb70c8293f9ca42ea3e448327fc50
PKG_HASH:=71b2c3d1cd26ed1ec7c8196834143258b2ad7f444efff26fdc366c6f5e752702

PKG_BUILD_DIR:=$(BUILD_DIR)/protobuf-$(PKG_VERSION)

PKG_MAINTAINER:=Philippe BIONDI <guillaume@valadon.net>
PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=LICENSE

HOST_PYTHON3_PACKAGE_BUILD_DEPENDS:=Cython

include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-protobuf
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:=Scipy
  DEPENDS:=+python3-light
  VARIANT:=python3
endef

define Package/python3-protobuf/description
  Composable command line interface toolkit
endef

$(eval $(call Py3Package,python3-protobuf))
$(eval $(call BuildPackage,python3-protobuf))
$(eval $(call BuildPackage,python3-protobuf-src))
