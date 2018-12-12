include $(TOPDIR)/rules.mk

PKG_NAME:=ffka-domain-migrator
PKG_VERSION:=2
PKG_RELEASE:=1

include $(TOPDIR)/../package/gluon.mk

define Package/ffka-domain-migrator
  TITLE:=ffka-domain-migrator
  DEPENDS:=+gluon-core
endef

$(eval $(call BuildPackageGluon,ffka-domain-migrator))
