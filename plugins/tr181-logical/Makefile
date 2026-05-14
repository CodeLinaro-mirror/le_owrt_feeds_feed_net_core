# WARNING: Automatically generated file using BAF (Build system Agnostic File) tooling (version master)
# WARNING: You should contribute changes to https://gitlab.com/prpl-foundation/components/core/plugins/tr181-logical/-/blob/main/baf.yml instead
include $(TOPDIR)/rules.mk

PKG_NAME:=tr181-logical
RAW_VERSION:=sah-next-4.2_v1.0.0
PKG_VERSION:=$(if $(filter v0% v1% v2% v3% v4% v5% v6% v7% v8% v9%,$(RAW_VERSION)),$(patsubst v%,%,$(RAW_VERSION)),$(RAW_VERSION))
SHORT_DESCRIPTION:=logical interface plugin

PKG_SOURCE:=tr181-logical-sah-next-4.2_v1.0.0.tar.gz
PKG_SOURCE_URL:=https://gitlab.com/prpl-foundation/components/core/plugins/tr181-logical/-/archive/sah-next-4.2_v1.0.0
PKG_HASH:=c5f6fb75907d41868f78b7e3e02d17780bc300c7d9eda278a0fedea854af0f72
PKG_BUILD_DIR:=$(BUILD_DIR)/tr181-logical-sah-next-4.2_v1.0.0
PKG_MAINTAINER:=Soft At Home <support.opensource@softathome.com>
PKG_LICENSE:=BSD-2-Clause-Patent
PKG_LICENSE_FILES:=LICENSE

COMPONENT:=tr181-logical

PKG_RELEASE:=1

define SAHInit/Install
	install -d $(1)/etc/rc.d/
ifneq ($(CONFIG_PACKAGE_procd),y)
	ln -sfr $(1)/etc/init.d/$(COMPONENT) $(1)/etc/rc.d/S$(CONFIG_SAH_AMX_TR181_LOGICAL_START_ORDER)$(COMPONENT)
	ln -sfr $(1)/etc/init.d/$(COMPONENT) $(1)/etc/rc.d/K$(CONFIG_SAH_AMX_TR181_LOGICAL_STOP_ORDER)$(COMPONENT)
endif
endef

include $(INCLUDE_DIR)/package.mk

define Package/$(PKG_NAME)
  CATEGORY:=prpl Foundation
  SUBMENU:=TR-181 Managers
  TITLE:=$(SHORT_DESCRIPTION)
  URL:=https://gitlab.com/prpl-foundation/components/core/plugins/tr181-logical
  DEPENDS += +libamxb
  DEPENDS += +libamxc
  DEPENDS += +libamxd
  DEPENDS += +libamxo
  DEPENDS += +libamxp
  DEPENDS += +libsahtrace
  DEPENDS += +libnetmodel
  DEPENDS += +amxrt
  DEPENDS += +mod-dmstats
  DEPENDS += +mod-netmodel
  MENU:=1
endef

define Package/$(PKG_NAME)/description
	logical interface plugin
endef

define Build/Compile
	$(call Build/Compile/Default, STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PKG_CONFIG_PATH=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_AMX_TR181_LOGICAL_START_ORDER=$(CONFIG_SAH_AMX_TR181_LOGICAL_START_ORDER) CONFIG_SAH_AMX_TR181_LOGICAL_STOP_ORDER=$(CONFIG_SAH_AMX_TR181_LOGICAL_STOP_ORDER) CONFIG_SAH_AMX_TR181_LOGICAL_RUN_AS_USER=$(CONFIG_SAH_AMX_TR181_LOGICAL_RUN_AS_USER) CONFIG_SAH_AMX_TR181_LOGICAL_RUN_AS_GROUP=$(CONFIG_SAH_AMX_TR181_LOGICAL_RUN_AS_GROUP) CONFIG_PRPL_CPE_OPMODE_EXTENDER=$(CONFIG_PRPL_CPE_OPMODE_EXTENDER) CONFIG_PRPL_CPE_OPMODE_GATEWAY=$(CONFIG_PRPL_CPE_OPMODE_GATEWAY) CONFIG_PACKAGE_procd=$(CONFIG_PACKAGE_procd))
endef

define Build/Install
	$(call Build/Install/Default, install INSTALL=install D=$(PKG_INSTALL_DIR) DEST=$(PKG_INSTALL_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(RAW_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_AMX_TR181_LOGICAL_START_ORDER=$(CONFIG_SAH_AMX_TR181_LOGICAL_START_ORDER) CONFIG_SAH_AMX_TR181_LOGICAL_STOP_ORDER=$(CONFIG_SAH_AMX_TR181_LOGICAL_STOP_ORDER) CONFIG_SAH_AMX_TR181_LOGICAL_RUN_AS_USER=$(CONFIG_SAH_AMX_TR181_LOGICAL_RUN_AS_USER) CONFIG_SAH_AMX_TR181_LOGICAL_RUN_AS_GROUP=$(CONFIG_SAH_AMX_TR181_LOGICAL_RUN_AS_GROUP) CONFIG_PRPL_CPE_OPMODE_EXTENDER=$(CONFIG_PRPL_CPE_OPMODE_EXTENDER) CONFIG_PRPL_CPE_OPMODE_GATEWAY=$(CONFIG_PRPL_CPE_OPMODE_GATEWAY) CONFIG_PACKAGE_procd=$(CONFIG_PACKAGE_procd))

	$(call SAHInit/Install,$(PKG_INSTALL_DIR))
endef

define Build/InstallDev
	$(call Build/Install/Default, install INSTALL=install D=$(STAGING_DIR) DEST=$(STAGING_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(RAW_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_AMX_TR181_LOGICAL_START_ORDER=$(CONFIG_SAH_AMX_TR181_LOGICAL_START_ORDER) CONFIG_SAH_AMX_TR181_LOGICAL_STOP_ORDER=$(CONFIG_SAH_AMX_TR181_LOGICAL_STOP_ORDER) CONFIG_SAH_AMX_TR181_LOGICAL_RUN_AS_USER=$(CONFIG_SAH_AMX_TR181_LOGICAL_RUN_AS_USER) CONFIG_SAH_AMX_TR181_LOGICAL_RUN_AS_GROUP=$(CONFIG_SAH_AMX_TR181_LOGICAL_RUN_AS_GROUP) CONFIG_PRPL_CPE_OPMODE_EXTENDER=$(CONFIG_PRPL_CPE_OPMODE_EXTENDER) CONFIG_PRPL_CPE_OPMODE_GATEWAY=$(CONFIG_PRPL_CPE_OPMODE_GATEWAY) CONFIG_PACKAGE_procd=$(CONFIG_PACKAGE_procd))
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
