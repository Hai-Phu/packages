# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=onnx
PKG_VERSION:=1.11.0
PKG_RELEASE:=1

PKG_SOURCE:=onnx-1.11.0.tar.gz
PKG_SOURCE_URL:=https://files.pythonhosted.org/packages/fd/b7/fccddff4d1873074605ff08acc812202b4a849cf4925b1f6ed5eeba575c4
PKG_HASH:=3bc63486a870294683980d76ec1e3efc786295ae00128f9ea38e2c6e74d5a60a

PKG_BUILD_DIR:=$(BUILD_DIR)/onnx-$(PKG_VERSION)

PKG_MAINTAINER:=Philippe BIONDI <guillaume@valadon.net>
PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=LICENSE

HOST_PYTHON3_PACKAGE_BUILD_DEPENDS:=Cython

include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-onnx
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:=Scipy
  DEPENDS:=+python3-light
  VARIANT:=python3
endef

define Package/python3-onnx/description
  Composable command line interface toolkit
endef

$(eval $(call Py3Package,python3-onnx))
$(eval $(call BuildPackage,python3-onnx))
$(eval $(call BuildPackage,python3-onnx-src))
