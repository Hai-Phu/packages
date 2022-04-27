# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=scikit-learn
PKG_VERSION:=0.24.2
PKG_RELEASE:=1

PKG_SOURCE:=scikit-learn-0.24.2.tar.gz
PKG_SOURCE_URL:=https://files.pythonhosted.org/packages/05/04/507280f20fafc8bc94b41e0592938c6f4a910d0e066be7c8ff1299628f5d
PKG_HASH:=d14701a12417930392cd3898e9646cf5670c190b933625ebe7511b1f7d7b8736

PKG_BUILD_DIR:=$(BUILD_DIR)/scikit-learn-$(PKG_VERSION)

PKG_MAINTAINER:=Daniel Golle <daniel@makrotopia.org>
PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=LICENSE

include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-scikit-learn
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:=scikit-learn
  DEPENDS:=+python3-light
  VARIANT:=python3
endef

define Package/python3-scikit-learn/description
  Composable command line interface toolkit
endef

$(eval $(call Py3Package,python3-scikit-learn))
$(eval $(call BuildPackage,python3-scikit-learn))
$(eval $(call BuildPackage,python3-scikit-learn-src))
