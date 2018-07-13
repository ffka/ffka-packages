include $(TOPDIR)/rules.mk

PKG_NAME:=ffka-domain-migrator
PKG_VERSION:=1
PKG_RELEASE:=1

PKG_BUILD_DIR := $(BUILD_DIR)/$(PKG_NAME)

include $(INCLUDE_DIR)/package.mk

define Package/ffka-domain-migrator
  SECTION:=gluon
  CATEGORY:=Gluon
  TITLE:=Migrate nodes to multidomain firmware
  DEPENDS:=+gluon-core micrond
endef

define Package/ffka-domain-migrator/description
	Migrate nodes to multidomain firmware and preserve domain information.
endef

define Build/Prepare
	mkdir -p $(PKG_BUILD_DIR)
	$(CP) ./src/* $(PKG_BUILD_DIR)/
endef

define Build/Configure
endef

define Build/Compile
	$(call Build/Compile/Default)
endef

define Package/ffka-domain-migrator/install
	$(CP) ./luasrc/* $(1)/
	$(CP) ./files/* $(1)/
endef

$(eval $(call BuildPackage,ffka-domain-migrator))
