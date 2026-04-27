# WARNING: Automatically generated file using BAF (Build system Agnostic File) tooling (version master)
# WARNING: You should contribute changes to https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dslite/-/blob/main/baf.yml instead
include $(TOPDIR)/rules.mk

PKG_NAME:=tr181-dslite
RAW_VERSION:=sah-next-4.1-lts_v0.2.0
PKG_VERSION:=$(if $(filter v0% v1% v2% v3% v4% v5% v6% v7% v8% v9%,$(RAW_VERSION)),$(patsubst v%,%,$(RAW_VERSION)),$(RAW_VERSION))
SHORT_DESCRIPTION:=TR-181 compatible DSLite plugin

PKG_SOURCE:=tr181-dslite-sah-next-4.1-lts_v0.2.0.tar.gz
PKG_SOURCE_URL:=https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dslite/-/archive/sah-next-4.1-lts_v0.2.0
PKG_HASH:=f951f4321a062972c88ab64f6ef479824d2fc2e2f33575f4171f2640b912788b
PKG_BUILD_DIR:=$(BUILD_DIR)/tr181-dslite-sah-next-4.1-lts_v0.2.0
PKG_MAINTAINER:=Soft At Home <support.opensource@softathome.com>
PKG_LICENSE:=BSD-2-Clause-Patent
PKG_LICENSE_FILES:=LICENSE

COMPONENT:=tr181-dslite

PKG_RELEASE:=1

define SAHInit/Install
	install -d $(1)/etc/rc.d/
	ln -sfr $(1)/etc/init.d/$(COMPONENT) $(1)/etc/rc.d/S$(CONFIG_SAH_AMX_TR181_DSLITE_START_ORDER)$(COMPONENT)
	ln -sfr $(1)/etc/init.d/$(COMPONENT) $(1)/etc/rc.d/K$(CONFIG_SAH_AMX_TR181_DSLITE_STOP_ORDER)$(COMPONENT)
endef

include $(INCLUDE_DIR)/package.mk

define Package/$(PKG_NAME)
  CATEGORY:=prpl Foundation
  SUBMENU:=Ambiorix
  TITLE:=$(SHORT_DESCRIPTION)
  URL:=https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dslite
  DEPENDS += +libamxc
  DEPENDS += +libamxp
  DEPENDS += +libamxd
  DEPENDS += +libamxo
  DEPENDS += +libamxm
  DEPENDS += +libamxb
  DEPENDS += +libsahtrace
  DEPENDS += +amxrt
  DEPENDS += +mod-netmodel
  DEPENDS += +libnetmodel
  DEPENDS += +libcares
  DEPENDS += +kmod-ip6-tunnel
  DEPENDS += +kmod-iptunnel6
  MENU:=1
endef

define Package/$(PKG_NAME)/description
	TR-181 compatible DSLite plugin
endef

define Build/Compile
	$(call Build/Compile/Default, STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PKG_CONFIG_PATH=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_AMX_TR181_DSLITE_START_ORDER=$(CONFIG_SAH_AMX_TR181_DSLITE_START_ORDER) CONFIG_SAH_AMX_TR181_DSLITE_STOP_ORDER=$(CONFIG_SAH_AMX_TR181_DSLITE_STOP_ORDER) CONFIG_SAH_AMX_TR181_DSLITE_CARES_RPATH=$(CONFIG_SAH_AMX_TR181_DSLITE_CARES_RPATH) CONFIG_SAH_AMX_TR181_DSLITE_RUN_AS_USER=$(CONFIG_SAH_AMX_TR181_DSLITE_RUN_AS_USER) CONFIG_SAH_AMX_TR181_DSLITE_RUN_AS_GROUP=$(CONFIG_SAH_AMX_TR181_DSLITE_RUN_AS_GROUP))
endef

define Build/Install
	$(call Build/Install/Default, install INSTALL=install D=$(PKG_INSTALL_DIR) DEST=$(PKG_INSTALL_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(RAW_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_AMX_TR181_DSLITE_START_ORDER=$(CONFIG_SAH_AMX_TR181_DSLITE_START_ORDER) CONFIG_SAH_AMX_TR181_DSLITE_STOP_ORDER=$(CONFIG_SAH_AMX_TR181_DSLITE_STOP_ORDER) CONFIG_SAH_AMX_TR181_DSLITE_CARES_RPATH=$(CONFIG_SAH_AMX_TR181_DSLITE_CARES_RPATH) CONFIG_SAH_AMX_TR181_DSLITE_RUN_AS_USER=$(CONFIG_SAH_AMX_TR181_DSLITE_RUN_AS_USER) CONFIG_SAH_AMX_TR181_DSLITE_RUN_AS_GROUP=$(CONFIG_SAH_AMX_TR181_DSLITE_RUN_AS_GROUP))

	$(call SAHInit/Install,$(PKG_INSTALL_DIR))
endef

define Build/InstallDev
	$(call Build/Install/Default, install INSTALL=install D=$(STAGING_DIR) DEST=$(STAGING_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(RAW_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_AMX_TR181_DSLITE_START_ORDER=$(CONFIG_SAH_AMX_TR181_DSLITE_START_ORDER) CONFIG_SAH_AMX_TR181_DSLITE_STOP_ORDER=$(CONFIG_SAH_AMX_TR181_DSLITE_STOP_ORDER) CONFIG_SAH_AMX_TR181_DSLITE_CARES_RPATH=$(CONFIG_SAH_AMX_TR181_DSLITE_CARES_RPATH) CONFIG_SAH_AMX_TR181_DSLITE_RUN_AS_USER=$(CONFIG_SAH_AMX_TR181_DSLITE_RUN_AS_USER) CONFIG_SAH_AMX_TR181_DSLITE_RUN_AS_GROUP=$(CONFIG_SAH_AMX_TR181_DSLITE_RUN_AS_GROUP))
	$(call SAHInit/Install,$(STAGING_DIR))
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
