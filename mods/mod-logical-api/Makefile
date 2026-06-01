# WARNING: Automatically generated file using BAF (Build system Agnostic File) tooling (version master)
# WARNING: You should contribute changes to https://gitlab.com/prpl-foundation/components/core/modules/mod-logical-api/-/blob/main/baf.yml instead
include $(TOPDIR)/rules.mk

PKG_NAME:=mod-logical-api
RAW_VERSION:=sah-next-4.2_v0.1.0
PKG_VERSION:=$(if $(filter v0% v1% v2% v3% v4% v5% v6% v7% v8% v9%,$(RAW_VERSION)),$(patsubst v%,%,$(RAW_VERSION)),$(RAW_VERSION))
SHORT_DESCRIPTION:=High Level API for configuring interface hierarchies

PKG_SOURCE:=mod-logical-api-sah-next-4.2_v0.1.0.tar.gz
PKG_SOURCE_URL:=https://gitlab.com/prpl-foundation/components/core/modules/mod-logical-api/-/archive/sah-next-4.2_v0.1.0
PKG_HASH:=8bfa867723512036874d5c5a707e922e9b88a7202bf68c09ec8fbe406f11d974
PKG_BUILD_DIR:=$(BUILD_DIR)/mod-logical-api-sah-next-4.2_v0.1.0
PKG_MAINTAINER:=Soft At Home <support.opensource@softathome.com>
PKG_LICENSE:=BSD-2-Clause-Patent
PKG_LICENSE_FILES:=LICENSE


PKG_RELEASE:=1

include $(INCLUDE_DIR)/package.mk

define Package/$(PKG_NAME)
  CATEGORY:=prpl Foundation
  SUBMENU:=Modules
  TITLE:=$(SHORT_DESCRIPTION)
  URL:=https://gitlab.com/prpl-foundation/components/core/modules/mod-logical-api
  DEPENDS += +libamxc
  DEPENDS += +libamxj
  DEPENDS += +libamxm
  DEPENDS += +libamxo
  DEPENDS += +libamxp
  DEPENDS += +libamxb
  DEPENDS += +libamxd
  DEPENDS += +libsahtrace
  DEPENDS += +libnetmodel
  DEPENDS += +libipat
  DEPENDS += +libdhcpoptions
  DEPENDS += +libipat
  MENU:=1
endef

define Package/$(PKG_NAME)/description
	High Level API for configuring interface hierarchies
endef

define Build/Compile
	$(call Build/Compile/Default, STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PKG_CONFIG_PATH=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_MOD_LOGICAL_API_LOGICAL_KICKSTATIONS_SUPPORTED=$(CONFIG_SAH_MOD_LOGICAL_API_LOGICAL_KICKSTATIONS_SUPPORTED) CONFIG_SAH_MOD_LOGICAL_API_LEGACY_SUPPORT=$(CONFIG_SAH_MOD_LOGICAL_API_LEGACY_SUPPORT))
endef

define Build/Install
	$(call Build/Install/Default, install INSTALL=install D=$(PKG_INSTALL_DIR) DEST=$(PKG_INSTALL_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(RAW_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_MOD_LOGICAL_API_LOGICAL_KICKSTATIONS_SUPPORTED=$(CONFIG_SAH_MOD_LOGICAL_API_LOGICAL_KICKSTATIONS_SUPPORTED) CONFIG_SAH_MOD_LOGICAL_API_LEGACY_SUPPORT=$(CONFIG_SAH_MOD_LOGICAL_API_LEGACY_SUPPORT))
endef

define Build/InstallDev
	$(call Build/Install/Default, install INSTALL=install D=$(STAGING_DIR) DEST=$(STAGING_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(RAW_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_MOD_LOGICAL_API_LOGICAL_KICKSTATIONS_SUPPORTED=$(CONFIG_SAH_MOD_LOGICAL_API_LOGICAL_KICKSTATIONS_SUPPORTED) CONFIG_SAH_MOD_LOGICAL_API_LEGACY_SUPPORT=$(CONFIG_SAH_MOD_LOGICAL_API_LEGACY_SUPPORT))
endef

define Package/$(PKG_NAME)/install
	if [ -d $(PKG_INSTALL_DIR) ]; then \
		$(CP) $(PKG_INSTALL_DIR)/* $(1)/; \
	fi
	if [ -d ./files ]; then \
		$(CP) ./files/* $(1)/; \
	fi
	find $(1) -name *.a -exec rm {} +;
	find $(1) -name *.h -exec rm {} +;
	find $(1) -name *.pc -exec rm {} +;
endef

define Package/$(PKG_NAME)/config
	source "$(SOURCE)/Config.in"
endef

$(eval $(call BuildPackage,$(PKG_NAME)))
