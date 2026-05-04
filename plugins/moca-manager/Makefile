# WARNING: Automatically generated file using BAF (Build system Agnostic File) tooling (version 2.40.6)
# WARNING: You should contribute changes to https://gitlab.com/prpl-foundation/components/core/plugins/tr181-moca/-/blob/main/baf.yml instead
include $(TOPDIR)/rules.mk

PKG_NAME:=moca-manager
RAW_VERSION:=sah-next-4.1_v3.4.0
PKG_VERSION:=$(if $(filter v0% v1% v2% v3% v4% v5% v6% v7% v8% v9%,$(RAW_VERSION)),$(patsubst v%,%,$(RAW_VERSION)),$(RAW_VERSION))
SHORT_DESCRIPTION:=MoCA plugin

PKG_SOURCE:=tr181-moca-sah-next-4.1_v3.4.0.tar.gz
PKG_SOURCE_URL:=https://gitlab.com/prpl-foundation/components/core/plugins/tr181-moca/-/archive/sah-next-4.1_v3.4.0
PKG_HASH:=4f9b7942857b2403dc8e1135b0184d52f3476aa40d21be0886f75a3bbe6311aa
PKG_BUILD_DIR:=$(BUILD_DIR)/tr181-moca-sah-next-4.1_v3.4.0
PKG_MAINTAINER:=Soft At Home <support.opensource@softathome.com>
PKG_LICENSE:=BSD-2-Clause-Patent
PKG_LICENSE_FILES:=LICENSE

COMPONENT:=moca-manager

PKG_RELEASE:=1

define SAHInit/Install
	install -d $(1)/etc/rc.d/
	ln -sfr $(1)/etc/init.d/$(COMPONENT) $(1)/etc/rc.d/S$(CONFIG_SAH_AMX_TR181_MOCA_ORDER)$(COMPONENT)
	ln -sfr $(1)/etc/init.d/$(COMPONENT) $(1)/etc/rc.d/K$(CONFIG_SAH_AMX_TR181_MOCA_STOP_ORDER)$(COMPONENT)
endef

include $(INCLUDE_DIR)/package.mk

define Package/$(PKG_NAME)
  CATEGORY:=prpl Foundation
  SUBMENU:=TR-181 Managers
  TITLE:=$(SHORT_DESCRIPTION)
  URL:=https://gitlab.com/prpl-foundation/components/core/plugins/tr181-moca
  DEPENDS += +libamxb
  DEPENDS += +libamxc
  DEPENDS += +libamxd
  DEPENDS += +libamxm
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
	MoCA plugin
endef

define Build/Compile
	$(call Build/Compile/Default, STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PKG_CONFIG_PATH=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_AMX_TR181_MOCA_ORDER=$(CONFIG_SAH_AMX_TR181_MOCA_ORDER) CONFIG_SAH_AMX_TR181_MOCA_STOP_ORDER=$(CONFIG_SAH_AMX_TR181_MOCA_STOP_ORDER))
endef

define Build/Install
	$(call Build/Install/Default, install INSTALL=install D=$(PKG_INSTALL_DIR) DEST=$(PKG_INSTALL_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(RAW_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_AMX_TR181_MOCA_ORDER=$(CONFIG_SAH_AMX_TR181_MOCA_ORDER) CONFIG_SAH_AMX_TR181_MOCA_STOP_ORDER=$(CONFIG_SAH_AMX_TR181_MOCA_STOP_ORDER))

	$(call SAHInit/Install,$(PKG_INSTALL_DIR))
endef

define Build/InstallDev
	$(call Build/Install/Default, install INSTALL=install D=$(STAGING_DIR) DEST=$(STAGING_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(RAW_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_AMX_TR181_MOCA_ORDER=$(CONFIG_SAH_AMX_TR181_MOCA_ORDER) CONFIG_SAH_AMX_TR181_MOCA_STOP_ORDER=$(CONFIG_SAH_AMX_TR181_MOCA_STOP_ORDER))
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
