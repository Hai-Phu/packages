# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=Theano
PKG_VERSION:=1.0.5
PKG_RELEASE:=1

PKG_SOURCE:=Theano-1.0.5.tar.gz
PKG_SOURCE_URL:=https://files.pythonhosted.org/packages/6b/97/bcd5654ba60f35f180931afabbd3b4c46c0379852f961c7a2819ff897f5d
PKG_HASH:=6e9439dd53ba995fcae27bf20626074bfc2fff446899dc5c53cb28c1f9202e89

PKG_BUILD_DIR:=$(BUILD_DIR)/Theano-$(PKG_VERSION)

PKG_MAINTAINER:=Philippe BIONDI <guillaume@valadon.net>
PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=LICENSE

HOST_PYTHON3_PACKAGE_BUILD_DEPENDS:=Cython

include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-Theano
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:=Scipy
  DEPENDS:=+python3-light
  VARIANT:=python3
endef

define Package/python3-Theano/description
  Composable command line interface toolkit
endef

$(eval $(call Py3Package,python3-Theano))
$(eval $(call BuildPackage,python3-Theano))
$(eval $(call BuildPackage,python3-Theano-src))
